# Formatando o cartão SD (Windows)

## Leitura Obrigatória

Essa é uma seção adicional para a formatação de um cartão SD para fazê-lo funcional com o 3DS.

Se o 3DS já reconhece o cartão SD, este guia não é necessário.

Esta página é destinada apenas a usuários do Windows. Caso você não esteja usando Windows, acesse a página [Formatando SD (Linux)](formatting-sd-(linux)) ou [Formatando SD (Mac)](formatting-sd-(mac))

## O que é necessário

- The latest version of [guiformat](https://nintendohomebrew.com/guiformat)

## Instruções

1. Execute `guiformat.exe`

2. Selecione a letra da unidade do seu cartão SD em "Drive"

   ::: danger

   Certifique-se de escolher a letra da unidade correta, caso contrário você pode apagar a unidade errada acidentalmente!

   :::

3. Selecione um tamanho para "Allocation unit size"
   - Se o cartão SD for de 64GB, escolha 32768
   - Se o cartão SD for maior que 64GB, escolha 65536

4. Digite qualquer coisa para "Volume label"

5. Certifique-se de que "Quick Format" está selecionado

6. Clique em "Start"

7. Clique em "OK"

8. Aguarde a conclusão da formatação

9. Clique em "Close"

10. Se o cartão SD tinha quaisquer arquivos ou pastas nele, copie tudo de volta para o SD do seu computador

## Troubleshooting

- guiformat mostra o erro "Failed to open device: GetLastError()=32"
  - Feche tudo o que estiver usando o cartão SD, como qualquer janela do Explorador de Arquivos.
  - Se este problema persistir, tente reformatar o cartão para NTFS no Gerenciador de Arquivos, feche essa janela quando terminar, e tente novamente o processo do guiformat.

- guiformat mostra o erro "GetLastError()=1117"
  - A chave contra proteção de escrita no cartão SD pode estar [habilitada](/images/sdlock.png). A chave deve ser virada para cima para permitir a escrita de arquivos no cartão SD (incluindo formatação).

- O cartão SD permanece não sendo detectado pelo console, ou continua mostrando a capacidade errada após a formatação
  - Seu cartão SD pode estar particionado ou ter espaço não alocado. Siga as instruções [aqui](https://wiki.hacks.guide/wiki/SD_Clean/Windows) para reformatar o seu cartão SD.
