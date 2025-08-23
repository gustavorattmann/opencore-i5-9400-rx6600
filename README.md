# Opencore Intel I5 9400 AMD Radeon RX 6600 8GB

## O que é Hackintosh?

É a preparação de um computador que não seja criado pela Apple para instalação do sistema operacional Mac.

## O que é Opencore?

É responsável por fazer a configuração que permitirá o Mac reconhecer os dispositivos do seu computador e fazer com que eles trabalhem da forma espereda.

**Nota:** Para configurar o Opencore é necessário esforço, tempo, dedicação e aprendizado, mas não é nada que seja de outro mundo.

É sempre importante consultar a documentação oficial ou procurar auxílio na internet, pois cada dispositivo tem sua própria configuração.

## Dica

A pouco tempo conheci uma ferramenta maravilhosa chamada OpCore Simplify, que cria a EFI com base em seu Windows, detectando seu hardware... Se seu hardware possui algumas diferenças do meu, aconselho a criar sua EFI com base nessa ferramenta. Há vários tutoriais de como utilizá-la, depois é só fazer os ajustes finais.

Mantenha sempre um backup da útlima versão do Opencore que você criar ou alterar em um pen drive, para prevenção e manutenção, além de armazenar em nuvem, sempre que precisar recuperar.

Faça uma análise nas pastas de Kexts, ACPI e drivers e remova o que não for utilizar, depois faça um snapshot na configuração do OC para atualizar apenas com o que manteve. Esse passo também deve ser feito se adicionar algum novo.

Outro ajuste necessário é adicionar uma SMBIOS válida para permitir que algumas funcionalidades executem da forma correta como FaceTime e Mensagens.

**Nota:** Caso utilize algum SSD NVME da Samsung, poderá enfrentar lentidão durante o boot... Para resolver precisa alterar o valor da propriedade "**SetApfsTrimTimeout**" de "**-1**" para "**0**" (No meu caso o tempo de boot que era cerca de 1 minuto caiu para 15 segundos).

## Versão do Opencore

1.0.5

## Minha Versão do Mac

Sequoia (15.5)

## Versão mínima compatível com Mac

Monterey (12.1)

## Meu Hardware

- Processador: Intel Core i5 9400 Hexa-Core 2.9 Ghz
- Memória: 2x8Gb Corsair Vengeance LPX 2666mhz
- Placa-mãe: ASUS TUF B360M-Plus Gaming/BR
- Placa de vídeo: AMD Radeon XFX Swft 210 RX 6600 8Gb
- Fonte: Corsair CV650 80 Plus Bronze - 650 Watts
- Armazenamento: SSD NVMe Samsung 970 EVO Plus 500Gb (MacOS Sequoia)
- SSD NVMe Kingspec 512Gb (Windows)
- SSD Sata SanDisk 240Gb 2,5" (Linux)
- HD Western Digital 1Tb 3,5" (500Gb de Backup do MacOS/500Gb do diretório Home do Linux)
- Cooler: Deep Cooler Gammaxx GTE V2
- Ventoinhas: 5x Pichau Gaming Wave 120R Led Vermelho
- Controlador de fan: DeepCool FH-10 PWM
- Gabinete: Cougar Gemini M Iron Gray

## Programas essenciais

[Opencore Configurator](https://mackie100projects.altervista.org/download/occ/) - Para configuração dinâmica do arquivo de extensão plist

[Hackintool](https://github.com/benbaker76/Hackintool) - Ferramenta essencial para ajudar na configuração e também para fazer patches

[Kext Updater](https://update.kextupdater.de/kextupdater/Kext%20Updater.zip) - Responsável por baixar o Opencore e as kexts quando precisarem ser atualizados

[ProperTree](https://github.com/corpnewt/ProperTree) - Para configuração de texto do arquivo de extensão plist

[MaciASL](https://github.com/acidanthera/MaciASL) - Para auxiliar a criar os patches de SSDT

[IORegistery](https://github.com/khronokernel/IORegistryClone) - Obter informações de hardware no Mac em tempo real

[OpCore Simplify](https://github.com/lzhoang2801/OpCore-Simplify) - A melhor ferramenta para criar uma EFI pelo Windows de forma automática (Facilita cerca de 90% do processo)

## Links de auxílio

[Documentação oficial](https://dortania.github.io/OpenCore-Install-Guide/)

[Grupo Hackintosh Brasil - Facebook](https://www.facebook.com/groups/hackintoshbrazil)

[Canal do Gabriel Luchina](https://www.youtube.com/@UniversoHackintosh)

[Canal do Dicas do Mateus](https://www.youtube.com/@DicasdoMateus)
