# Formatting SD (Windows)

## Required Reading

Dit is een extra sectie voor het formatteren van een SD-kaart om deze te doen werken met een 3DS-systeem.

Als de 3DS de SD kaart al herkent, is deze handleiding niet nodig.

Deze pagina is alleen voor windows-gebruikers. Als je geen Windows gebruikt, bekijk dan de [SD formatteren (Linux)](formatting-sd-(linux)) of [SD formatteren (Mac)](formatting-sd-(mac)) pagina's.

## What You Need

- The latest version of [guiformat](https://nintendohomebrew.com/guiformat)

## Instructions

1. Run `guiformat.exe`

2. Select your SD card's drive letter for "Drive"

   ::: danger

   Zorg ervoor dat je de juiste stationsletter kiest, anders kan je per ongeluk de verkeerde schijf verwijderen!

   :::

3. Select a size for "Allocation unit size"
   - If the SD card is 64GB, choose 32768
   - If the SD card is larger than 64GB, choose 65536

4. Voer iets in voor "Volume label"

5. Zorg ervoor dat "Quick Format" is geselecteerd

6. Click "Start"

7. Klik op "OK"

8. Wacht tot het formatteren is voltooid

9. Klik op "Close"

10. Als de SD-kaart al bestanden en mappen voor het formatteren bevatte, kopieer dan alles terug van uw computer

## Probleemoplossing

- guiformat shows the error "Failed to open device: GetLastError()=32"
  - Close everything that may be using the SD card, such as any File Explorer windows.
  - If this issue persists, try reformatting the card to NTFS in File Explorer, close that window when it's done, and re-attempt the guiformat process.

- guiformat shows the error "GetLastError()=1117"
  - Your SD card write-protection switch may be [enabled](/images/sdlock.png). The lock must be flipped upwards to allow writing to the SD card (including formatting).

- SD card remains undetected by console or continues to display the wrong capacity after formatting
  - Your SD card may be partitioned or have unallocated space. Follow the instructions [here](https://wiki.hacks.guide/wiki/SD_Clean/Windows) to reformat your SD card.
