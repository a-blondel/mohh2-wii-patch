# Patches for Medal Of Honor Heroes 2 [Wii]

A project dedicated to connect the game to a private server, as well as some features.

Our implementation of the private server can be found here : https://github.com/a-blondel/mohh2-wii-server


## Riivolution patches and Gecko Codes

**Riivolution** patches are made for Dolphin only, as the Riivolution homebrew doesn't work with MoHH2 on Wii. **Gecko Codes** is a fallback solution for the Wii.

The patches target the following versions of MoHH2 :
- RM2P69 : PAL UK
- RM2X69 : PAL EU (Fr,De,It,Es)
- RM2E69 : NTSC US
- RM2E69-beta : NTSC US (Oct 17, 2007 prototype)

### Available patches

- **Private Server**
  - **WFC replacement** : Required to access the private server. On Wii you can use the `Private Server` feature of USB Loader GX (recent versions only). Two options supported :
    - NoSSL - Requires to host a [NWC server](https://github.com/a-blondel/nwc-server)
	- Wiimmfi
  - **Serverless** : Allows to start a game alone without a working UDP server. **Beware : it crashes when taking damage !**
- **Mods**
  - **Online Panzerschreck** : Restores the panzerschreck for the germans (which was replaced by the M1 Bazooka on the Wii version while being available on the PSP version)  

<img src="doc/img/panzerschreck-label.png" alt="panzerschreck-label" width="400"/> <img src="doc/img/panzerschreck.png" alt="panzerschreck" width="400"/><br/>
*Panzerschreck label / ingame*
- **Misc**
  - **Menu Theme** : Change the theme menu, optional.
  - **Skip startup screens** : Skips the Wiimote and Zii Zapper alert screens on game startup to spare some time, optional.
  - **Skip EA intro** : Skips the intro to spare some time, optional.


### Usage

- Dolphin
  - Copy and Paste content of the `Riivolution` folder inside of your `Dolphin/User/Load/Riivolution` folder.
  - Right click on the game, click on `Start with Riivolution Patches`, click on `Open Riivolution XML...` and select the XML related to your version of the game.
  - Activate the patches you need.
- Wii
  - Two options to apply the codes :
    - Copy the .txt file matching your Game ID from the `GeckoCodes` folder, and paste it in a folder named `txtcodes` at the root of your SD card. Then in your game loader go to `game settings`, `ocarina`, activate the codes you want, and click create. Don't forget to enable Ocarina in the Game Load setting. This option is more flexible as you can quickly change the codes on the Wii.
    - Generate a GCT file based on the .txt file matching your Game ID from the `GeckoCodes` folder, then put the gct file in a `codes` folder at the root of your SD card. There are many sites and applications to create GCT files. If you feel nostlagic you might want to try my static version of [GeckoCodes.org](https://a-blondel.github.io/geckocodes.org/gct.html) ! Don't forget to enable Ocarina in the Game Load setting.


## Symbols map

If needed, please check the `symbols-map` folder.
