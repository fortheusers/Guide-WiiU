# CBHC

## Preparazione Della SD {docsify-ignore}

Ora inseriremo i file CFW richiesti e alcuni altri file homebrew sulla scheda SD.

?> **Nota Bene** La tua SD dovrà essere formattata in FAT32. Se la tua SD non è formattata in FAT32 usa [GUIFormat](http://ridgecrop.co.uk/index.htm?guiformat.htm) con 32k (32768) di Unità di allocazione per formattarla. **Non** chiamare la SD come `wiiu` o causerà problemi con homebrew.

### Cosa Ti Servirà {docsify-ignore}

- La versione più recente di [Homebrew Launcher Installer](https://github.com/wiiu-env/homebrew_launcher_installer/releases/latest).
  - Dovrai installare il file `payload.zip`.
- La versione 1.4 di [The Homebrew Launcher](https://github.com/dimok789/homebrew_launcher/releases/tag/1.4).
  - Dovrai installare la versione 1.4 `homebrew_launcher.v1.4.zip` dell' Homebrew Launcher.
- La versione più recente di [WUP Installer GX2](https://wiiubru.com/appstore/zips/wup_installer_gx2.zip).
- La versione più recente di [Homebrew Launcher Channel](https://github.com/GaryOderNichts/homebrew_launcher/releases/tag/v2.1_fix).
  - Dovrai installare il file `homebrew_launcher_channel.v2.1_fix.zip`.
- La versione più recente di [Wii U NAND Dumper](https://www.wiiubru.com/appstore/zips/nanddumper.zip).
- La versione più recente dell'[Homebrew App Store](https://github.com/vgmoose/hbas/releases/latest).
  - Dovrai installare il file `wiiu-extracttosd.zip`.
- La versione più recente di [Haxchi](https://www.wiiubru.com/appstore/zips/haxchi.zip).
- La versione più recente di [CBHC](https://www.wiiubru.com/appstore/zips/cbhc.zip).
- La versione più recente di <a href="docs/files/SaveMii_Mod.zip" download>SaveMii Mod</a>.

### Istruzioni {docsify-ignore}

?> **Nota Bene** I file info.json e manifest.install non servono per la modifica e quindi possono essere eliminati.

1. Inserisci la SD della tua Wii U nel PC.
1. Crea una cartella chiamata `install` nella root della tua SD.
1. Copia i contenuti di `homebrew_launcher_channel.v2.1_fix.zip` nella cartella `install` che hai creato precedentemente.
1. Copia i contenuti del file `haxchi.zip` nella root della tua SD.
1. Copia i contenuti del file `cbhc.zip` nella root della tua SD.
1. Copia i contenuti di `wup_installer_gx2.zip` nella root della tua SD.
1. Copia i contenuti del file `nanddumper.zip` nella root della tua SD.
1. Copia i contenuti del file `wiiu-extracttosd.zip` nella root della tua SD.
1. Copia i contenuti del file `homebrew_launcher.v.1.4.zip` nella root della tua SD.
1. Copia i contenuti del file `savemii_mod.zip` nella root della tua SD.
1. Copia il `payload.elf` dal `payload.zip` nella cartella `wiiu`.
----------

### Layout scheda SD {docsify-ignore}

<details>
<summary>Clicca qui per mostrare il layout finale della scheda SD.</summary>

```
💾sd:
 ┣ 📂cbhc
 ┃ ┣ 📜bootDrcTex.tga
 ┃ ┣ 📜bootTvTex.tga
 ┃ ┣ 📜iconTex.tga
 ┃ ┗ 📜title.txt
 ┣ 📂haxchi
 ┃ ┣ 📜bootDrcTex.tga
 ┃ ┣ 📜bootTvTex.tga
 ┃ ┣ 📜config.txt
 ┃ ┣ 📜iconTex.tga
 ┃ ┗ 📜title.txt
 ┣ 📂install
 ┃ ┗ 📂Homebrew Launcher Channel
 ┃   ┣ 📜00000000.app
 ┃   ┣ 📜00000003.h3
 ┃   ┣ ...
 ┃   ┣ 📜title.cert
 ┃   ┣ 📜title.tik
 ┃   ┗ 📜title.tmd
 ┗ 📂wiiu
   ┣ 📂apps
   ┃ ┣ 📂homebrew_launcher
   ┃ ┃ ┣ 📜homebrew_launcher.elf
   ┃ ┃ ┣ 📜icon.png
   ┃ ┃ ┗ 📜meta.xml
   ┃ ┗ (Anche tutte le altre app come disc2app, nanddumper, ecc. dovrebbero essere qui)
   ┗ 📜payload.elf
```

</details>
