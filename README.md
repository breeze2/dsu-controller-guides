# DSUController Guides

DSUController (means DualShock UDP controller) is a mobile app based on [cemuhook-protocol](https://github.com/v1993/cemuhook-protocol) to simulate some game controllers.
It can be used with [Cemu](http://cemu.info/) using [Cemuhook](https://sshnuke.net/cemuhook/), [Citra](https://citra-emu.org/), [Dolphin](https://dolphin-emu.org/), [Yuzu](https://yuzu-emu.org/) and other more game console emulators.

## Download

<a href='https://play.google.com/store/apps/details?id=com.dsucontroller&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png' style="height: 124px; object-position: -20px 20px;" /></a>
<br/>
<a href="https://apps.apple.com/us/app/dsucontroller/id1667281421?itsct=apps_box_badge&amp;itscg=30200" style="display: inline-block; overflow: hidden; border-radius: 13px; width: 250px; height: 83px;"><img src="https://tools.applemediaservices.com/api/badges/download-on-the-app-store/black/en-us?size=250x83&amp;releaseDate=1676505600" alt="Download on the App Store" style="border-radius: 13px; width: 250px; height: 83px;"></a>
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

    <img src="assets/dolphin/configure-controller.png" alt="Add DSU Client" width="640"/>

9. Close **Controller Settings** and start some games to have fun.
