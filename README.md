# DSUController Guides

DSUController (meaning DualShock UDP controller) is a mobile app based on [cemuhook-protocol](https://github.com/v1993/cemuhook-protocol) to simulate some game controllers.
It can be used with [Cemu](http://cemu.info/) using [Cemuhook](https://sshnuke.net/cemuhook/), [Citra](https://citra-emu.org/), [Dolphin](https://dolphin-emu.org/), [Yuzu](https://yuzu-emu.org/) and other more game console emulators.

## Screenshots

<img src="assets/dsu-controller/controller-page.png" alt="Controller Page" width="240"/>
<img src="assets/dsu-controller/settings-page.png" alt="Settings Page" width="240"/>

## Run with Dolphin

1. Open **Controller Settings** on Dolphin,
2. Click **Alternate Input Sources**,
3. Check **Enable**,
4. Click **Add...**, input the DSUController's IP address and port number (find them on the settings page),

    <img src="assets/dolphin/add-dsu-client.png" alt="Add DSU Client" width="640"/>

5. Select **Emulated Wii Remote** as `Wii Remote 1` and click **Configure**,
6. Select **Device** as `DSUClient/0/`,
7. Download <a href="configs/dolphin/DSUController.ini" download="DSUController.ini">DSUController.ini</a> into the Dolphin Config folder:
    > * windows: `~/Documents/Dolphin\ Emulator/Config/Profiles/Wiimote/`
    > * macOS: `~/Library/Application\ Support/Dolphin/Config/Profiles/Wiimote/`
8. Select **Profile** as `DSUController`, and click **load**,

    <img src="assets/dolphin/configure-controller.png" alt="Add DSU Client" width="640"/>

9. Close **Controller Settings** and start some games to have fun.
