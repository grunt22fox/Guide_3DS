# Formatting SD (Windows)

## Required Reading

这是一个适用于为 3DS 准备的 SD 卡的格式化教程。

如果 3DS 已经识别到了 SD 卡，那么就不需要做这个教程了。

本节教程仅限 Windows 用户。 如果你没有在用 Windows，那么请看看[格式化 SD 卡（通过 Linux 操作系统）](formatting-sd-(linux))或[格式化 SD 卡（通过 Mac 操作系统）](formatting-sd-(mac)) 。

## What You Need

- The latest version of [guiformat](https://nintendohomebrew.com/guiformat)

## Instructions

1. Run `guiformat.exe`

2. Select your SD card's drive letter for "Drive"

   ::: danger

   请确保你选对了驱动器盘符，否则你可能会把别的驱动器格式化了！

   :::

3. Select a size for "Allocation unit size"
   - If the SD card is 64GB, choose 32768
   - If the SD card is larger than 64GB, choose 65536

4. 在“Volume label”一行随便输入一些东西

5. 确保“Quick Format”被勾选

6. Click "Start"

7. 点击“OK”

8. 等待格式化完成

9. 点击“Close”

10. 如果先前你从 SD 卡上复制了一些文件或文件夹到电脑上，请将它们全部复制回 SD 卡

## 问题排查

- guiformat shows the error "Failed to open device: GetLastError()=32"
  - Close everything that may be using the SD card, such as any File Explorer windows.
  - If this issue persists, try reformatting the card to NTFS in File Explorer, close that window when it's done, and re-attempt the guiformat process.

- guiformat shows the error "GetLastError()=1117"
  - Your SD card write-protection switch may be [enabled](/images/sdlock.png). The lock must be flipped upwards to allow writing to the SD card (including formatting).

- SD card remains undetected by console or continues to display the wrong capacity after formatting
  - Your SD card may be partitioned or have unallocated space. Follow the instructions [here](https://wiki.hacks.guide/wiki/SD_Clean/Windows) to reformat your SD card.
