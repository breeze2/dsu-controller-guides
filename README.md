# DSUController Guides

DSUController (means DualShock UDP controller) is a mobile app based on [cemuhook-protocol](https://github.com/v1993/cemuhook-protocol) to simulate some game controllers.
It can be used with [Cemu](http://cemu.info/) using [Cemuhook](https://sshnuke.net/cemuhook/), [Citra](https://citra-emu.org/), [Dolphin](https://dolphin-emu.org/), [Yuzu](https://yuzu-emu.org/) and other more game console emulators.

## Download

<a href="https://play.google.com/store/apps/details?id=com.dsucontroller&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1" style="background: none; border: 1px solid #a6a6a6; border: 2px solid #a6a6a6; padding: 0; height: 84px; border-radius: 9px; display: inline-block;"><img src="./assets/badges/play-store.png" alt="Get it on Google Play" width="256" height="80" /></a>
<a href="https://apps.apple.com/us/app/dsucontroller/id1667281421?itsct=apps_box_badge&amp;itscg=30200" style="background: none; border: 1px solid #a6a6a6; border: 2px solid #a6a6a6; padding: 0; height: 84px; border-radius: 9px; display: inline-block;"><img src="./assets/badges/app-store.png" alt="Download on the App Store" width="256" height="80" /></a>
<br/>
<br/>

## Screenshots

<img src="assets/dsu-controller/controller-page.png" alt="Controller Page" width="240"/>
<img src="assets/dsu-controller/settings-page.png" alt="Settings Page" width="240"/>

## Run with Dolphin

1. Open **Controller Settings** on Dolphin,
2. Click **Alternate Input Sources**,
3. Check **Enable**,
4. Click **Add...**, input the DSUController's IP address and port number (find them on the settings page),

    <img src="assets/dolphin/add-dsu-client.png" alt="Add DSU Client" width="640"/>

5. Select `Emulated Wii Remote` as **Wii Remote 1** and click **Configure**,
6. Select `DSUClient/0/` as **Device**,
7. Download <a href="configs/dolphin/DSUController.ini" download="DSUController.ini">DSUController.ini</a> into the Dolphin Config folder:
    > * windows: `~/Documents/Dolphin\ Emulator/Config/Profiles/Wiimote/`
    > * macOS: `~/Library/Application\ Support/Dolphin/Config/Profiles/Wiimote/`
8. Select `DSUController` as **Profile**, and click **load**,

    <img src="assets/dolphin/configure-controller.png" alt="Configure Controller" width="640"/>

9. Close **Controller Settings** and start some games to have fun.

### FAQ

1. Why doesn't `DSUClient/x/` appear on Dolphin's Devices list?
    > Try to restart the DSU server or relaunch the app.<br />
    > Make sure the app and emulator are on the same Wi-Fi network, and [Local Network Access](https://support.apple.com/en-us/HT211870) is enabled on the app.
2. Can it rumble?
    > Yes, but the [PR](https://github.com/dolphin-emu/dolphin/pull/11545) for this feature is not merged currently.<br />
    > You can download the trial version of Dolphin Emulator from this [action artifacts](https://github.com/breeze2/dolphin/actions/runs/4314377128).<br />
    > Click **Motor**, and select `Motor 0` or `Motor 1` on **Configure Output** window. The phone will vibrate when you click **Test**.<br />
    > <img src="assets/dolphin/configure-motor.png" alt="Configure Motor" width="640"/>
3. Can it simulate Wii Nunchuk?
    > Yes, but you need two smartphones.<br />
    > First, download <a href="configs/dolphin/DSUController_with_Nunchuk.ini" download="DSUController_with_Nunchuk.ini">DSUController_with_Nunchuk.ini</a> into the Dolphin Config folder.<br />
    > Then select `DSUController_with_Nunchuk` as **Profile** on Dolphin Emulator controller settings window and load it.<br />
    > Make sure phone `DSUClient/0/` uses layout `Wii Remote` and phone `DSUClient/1/` uses layout `Wii Nunchuk` on DSUController settings page.<br />
    > <img src="assets/dsu-controller/controller-page-nunchuk.png" alt="Controller Page" width="240"/>
    > <img src="assets/dsu-controller/settings-page-nunchuk.png" alt="Settings Page" width="240"/>
4. Can it simulate Wii Classic Controller?
    > Yes.<br />
    > First, download <a href="configs/dolphin/DSUController_with_Classic.ini" download="DSUController_with_Classic.ini">DSUController_with_Classic.ini</a> into the Dolphin Config folder.<br />
    > Then select `DSUController_with_Classic` as **Profile** on Dolphin Emulator controller settings window and load it.<br />
    > When you touch `L` (or `R`), it will trigger the `L-Analog` (or `R-Analog`). Touch `L` (or `R`) and move out, it will trigger the real `L` (or `R`).<br />
    > <img src="assets/dsu-controller/controller-page-classic.png" alt="Controller Page" width="240"/>
    > <img src="assets/dsu-controller/settings-page-classic.png" alt="Settings Page" width="240"/>


## Privacy & Terms

- [Privacy](https://breeze2.github.io/dsu-controller-guides/privacy)
- [Terms & Conditions](https://breeze2.github.io/dsu-controller-guides/terms)