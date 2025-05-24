# Changelog
## (prior to wuMMLe)
</br>

## v1.1 (11/16/2020)
* Corrected FAVORIS to FAVORITE at the bottom of the screen when inside a system menu
* Added missing genesis folder to EASYROMS partition
* Fixed input not being shown when inserting username/password in scraper menu in default nes-box theme... (thanks to Jetup)
* Fixed the power led status (thanks to luali)
* Added support for Rumble (thanks to luali)
* Updated lr-pcsx_rearmed core with rumble support
* Added lr-flycast_rumble core with rumble support
* Added Amstrad CPC and Game and Watch retroarch cores and associated roms folders
* Added updated themes from Tiduscrying(gbz35 and gz35 dark mod) and Jetup(nes-box)
* Updated lr-mgba core with rumble support
* Updated options scripts to remove unnecessary screen outputs during loading
* Changed analog to digital setting for flycast to None
* Set analog sensitivity to 1.5
* Updated power led fix

## v1.1 (11/18/2020)
* Updated the power led fix to address an occasional issue that it may cause the gamepad controls to not be detected in Emulationstation and requiring a forced shutdown.  

## v1.1 (11/20/2020
* Updated mednafen_pce_fast libretro core to fix turbo button issue
* Updated Emulationstation to fix shift key character for builtin keyboard
* Updated boot text to reflect current version of ArkOS

## v1.2 (11/21/2020)
* Updated kernel to apply some realtek wireless chipset fixes.

## v1.2 (11/22/2020)
* Updated Retroarch to resolve an issue with loading remap files for fbneo core.
* Fix mastersystem scraper issue by renaming platform sms to mastersystem in es_systems.cfg

## v1.3 (11/23/2020)
* Updated kernel and modules adding support for additional rtl8812/rtl8821 based usb wifi dongles
* Updated dtbs to default clock speed to 1.3Ghz (Normal Clock) for stability and better consistent performance
* Added an Advanced option under the Options section
* Added ability to switch to 1.5Ghz (High Clock) from the Options/Advanced section
* Added ability to switch to 1.3Ghz (Normal Clock) from the Options/Advanced section
* Added ability to check current max speed from the Options/Advanced section
* Moved Fix ExFat Partition feature to Options/Advanced section
* Added zh-cn as a language locale for Emulationstation
* Updated Emulationstation to fix background music not returning after video screensaver stops
* Redirected background music folder to /roms/bgmusic folder for easier management
* Updated themes from Jetup (switch and epicnoir)

## v1.3 (11/24/2020)
* Updated Libretro Parallel_n64 core to support rumble.  See this FAQ entry on how to enable rumble: 
  (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-how-do-i-enable-rumblevibration-in-parallel_n64)
* Added support for the left analog stick for pico-8 (Thanks to fewt for finding the fix)
* Added the ability to enable and disable wifi in the Options/Advanced section.  
  This is for those who have internal wifi on their unit who wish to turn off wifi when not in use to help in saving power and heat generation.

## v1.3 (11/25/2020)
* Updated lr-mgba, lr-flycast_rumble, lr-parallel_n64, and lr-pcsx_rearmed cores with more efficient rumble support (Thanks to fewt for the idea)

## v1.3 (11/27/2020)
* Updated emulationstation adding a timezone setting in the start/advanced settings menu.
  - Be aware that when you hit A on the timezone menu option, it takes about 10 seconds or so for it to load and display all available timezones.  Please be patient.
* Updated retroarch32 to fix loading game, core, and content remap issues for some cores like lr-tyrquake
* Added Atari ST (lr-hatari) emulator
* Added Quake II (lr-vitaquake2) emulator for Quake II port
  - There's no support for music at this time until Libretro or the original developer of that emulator fixes this.
* Added support for recognizing .7z and .zip as supported file types for ZX Spectrum emulator.
* Updated the symlink for the Drastic emulator to the correct SDL2 library.

## v1.4 (11/29/2020)
* Updated initial boot expansion script for stability (Downloadable Image Only)
* Updated emulationstation fixing missing keyboard for creating custom game collections
* Added Backup settings and Restore settings function to Options/Advance section.  See FAQ #18 for more information about this feature.
* Added lr-puae as additional Amiga emulator
* Added standalone scummvm emulator

## v1.4 (12/01/2020)
* Reverted Dreamcast(lr-flycast-rumble), N64(lr-parallel-n64), and PSX (lr-pcsx-rearmed) cores to previous versions to restore performance
* Added support for Libretro Tic-80 emulator
* Updated themes from Jetup(nes-box, switch, epicnoir)
* Updated es_systems.cfg to address platform name for famicom to nes and sfc to snes to fix scraping and add tic-80 support

## v1.4 (12/03/2020)
* Reverted GBA (lr-mgba) core to previous version to restore stability
* Added Emulationstation menu translation for Portugal (Thanks to jonasbeavis)

## v1.4 (12/07/2020)
* Fixed some Emulationstation menu translations for Portuguese and Brazilian (Thanks to Leandro-Reis and jonasbeavis)
* Set resolution for Quake2 to 480x272 to fix initial performance if need be (Thanks to Gordon1972 and Jetup for confirmation)
* Added support for mapping the right analog stick in standalone ppsspp emulator
* Fixed the permission error for standalone ppsspp emulator
* Corrected supported extensions for MSX and MSX2 games
* Added bluemsx emulator option to Emulationstaton and defaulted MSX and MSX2 emulator to bluemsx instead (Thanks to Gordon1972 for testing and confirmation)
* Disabled systemd-resolved deamon to save on resources -- Reverted due to some losing internet after this update.
* Added ArkOS Browser (filebrowser) web file browser server.  Enabled when remote services are enabled.  
See FAQ #19 (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-how-do-i-use-arkos-browser-for-managing-my-roms-via-a-web-browser) 
on how to use this for managing roms via a web browser.

## v1.4 (12/09/2020)
* Added non rumble enabled GBA cores (MGBA, VBA-M, VBA-NExt)
* Ensure systemd-resolved has been reenabled

## v1.4 (12/12/2020)
* Added support for devilutionX port
* Updated platform names for Colecovision, Intellivision, and MSX2 to fix scraping
* Updated Backup Settings option to not include cheats and overlays to speed up the backup process

## v1.5 (12/15/2020)
* Installed updated SDL2 and graphics drivers and added Wayland to support various ports
* Installed image-viewer to support new splash screen
* Added Command Genius Port
* Added OpenTyrian Port
* Updated launch scripts to show splash screen before game launch if available
* Updated sources.list to fix apt-get since Ubuntu 19.10 EOAN is now End of Life
* Fixed L2 button for devilutionX port
* Really updated the Backup script this time to not include cheats and overlays to speed up backup and restore process.

## v1.5 (12/16/2020)
* Fixed bad update for German, Spanish and French ES Menu entries (Thanks to OolDEMool and olab75)
* Added update for a few themes to support Solarus and lzdoom system entries (Thanks to Jetup)
* Added support for Solarus
* Added lzdoom as default emulator for Doom wads as a new main system (former ports location will be deprecated in a future update)
(Thanks to That One Seong for the lzdoom port and tiduscrying for the lzdoom configuration)

## v1.5 (12/18/2020)
* Added support for RetroArch text-to-speech accessibility feature (Thanks to ridgekuhn for the suggestion and pull request)
* Added Tic-80 back to the ES Systems Menu 
* Added VVVVVV port

## v1.5 (12/19/2020)
* Updated PPSSPP emulator to 1.10.3 with batocera speedup.  (Thanks to fewt and batocera for patches)
* Updated lzdoom to swap OK and Cancel buttons.  (Thanks to That One Seong for the code changes and guidance)
* Updated Solarus to center image on screen.

## v1.5 (12/19/2020-1)
* Reverted PPSSPP emulator to previos PPSSPP-GO version.

## v1.5 (12/21/2020)
* Readded PPSSPPSDL 1.10.3 with fixed ppsspp.ini and keep original PPSSPPGO as additional emulator in Emulationstation
* Added glide64mk2 plugin for mupen64plus.  Selectable emulator named standalone-glide64mk2 in Emulationstation
* Updated lzdoom.ini to support Heretic, Hexen, Strife, and Chex Quest

## v1.5 (12/21/2020-1)
* Fixed Emulationstation menu for last update to recognize changes
Note: If you have specifically set up "standalone" for any of your N64 roms by editing the meta data, 
you'll need to update those rom settings to use either "standalone-Rice" or "standalone-Glide64mk2". 
For PSP, make sure you don't have a button assigned to speed toggle, atl speed 1 or alt speed 2. 
It's been reported that this causes major slowdowns with the new ppsspp emulator.

## v1.5 (12/22/2020) (Reenabled on 12/25/2020)
* Added support for Half-Life 1 port (Thanks to kreal for the conversion) 
(see https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#half-life-1 for proper instructions.)
* Added Prince of Persia port (Thanks to jetup)
* Added dosbox_pure libretro emulator as default dosbox core
* Power Led will turn red when battery life remaining is equal to or less than 30 percent
* Added exit key daemon for pico-8 (Select + Start will exit this game engine)
* Added exit key daemon for ppsspp-go (Select + Start will exit the emulator)
* Fixed solarus exit key daemon so that it will recover when exiting sleep mode during play

## v1.5 (12/26/2020)
* Added DinguxCommander File Manager
* Updated dtb to address possible occassional freezes during gameplay
* Added updated blacklist.conf file to stabilize rtl8xxx wifi chipsets
* Relocated Emulationstation themes to /roms/themes folder (if at least 1GB of space is available in EASYROMS partition)

## v1.5 (12/26/2020-1)
* Fix DinguxCommander File Manager control for rg351p

## v1.5 (12/27/2020)
* Updated emulationstation config file to add .m3u support for most CD based systems (AmigaCD, PC-Engine/TG16-CD, Sega CD, Dreamcast, DOS, etc.)
* Updated emulationstation config file to add support for .sh files for Doom system to support .pk3 mods.  
  Stay tuned to retrogamecorps for guides on this soon.
* Added updated blacklist to further mitigate performance issues for rtl8xxx chipsets (such as rtl8188CU and rtl8192cu) and resolve sleep issue.

## v1.5 (12/27/2020-1)
* Updated doom execution script to support running mod files using .sh extension

## v1.5 (01/02/2021)
* Updated emulationstation to fix display brightness decrement issue (Thanks to stino for assistance on this)
* Updated spanish translation for emulationstation (Thanks to Cisko for submission)
* Added Pokemon Mini system menu
* Added Atari Jaguar system menu - Performance is slow
* Added 3DO system menu - Performance is slow
* Fixed Atari 800, 5200 and XEGS rom loading issue due to options settings

## v1.5 (01/03/2021)
* Fixed Emulationstation platform and theme for Atari Jaguar
* Added support for .lha for Amiga CD32
* Added support for .zip for Pokemon Mini

## v1.5 (01/04/2021)
* Updated battery led script to blink red every 1 second when battery life is at 19% or lower.
* Added support for .zip for Amstrad CPC

## v1.5 (01/05/2021)
* Updated battery led script to fix excessive cpu usage
* Updated Retroarch and Retroarch32 with netplay fix
* Increase audio period and buffer sizes temporarily when running Drastic to improve performance

## v1.5 (01/09/2021)
* Fixed scraping for Neo-Geo CD
* Added support for .dim for x68000
* Added vmu to roms folder and background image to nes-box theme for vmu

## v1.5 (01/09/2021-1)
* Fixed scraping for Pokemon Mini

## v1.5 (01/10/2021)
* Added Daphne (Hypseus) emulator
  * for key assignments, see Daphne section within the rg351p global hotkey section of faq 
    (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-what-are-the-global-event-keys-and-emulator-event-keys-in-ArkOS)
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#daphne)
  
## v1.5 (01/11/2021)
* Changed opentyrian port to 32 bit to improve performance
* Added workaround for retroarch crashes when taking screenshots
* Added fix for shaders not autoloading when saved
* Added vibration support for Pokemon Mini emulator

## v1.5 (01/15/2021)
* Updated MGBA_Rumble core
* Updated Flycast_Rumble core (Previous savestates may not load with his updated rumble core)
* Updated PCSX_Rearmed_Rumble core and added as a separate core for psx

## v1.5 (01/16/2021)
* Added Uzebox (lr-uzem) emulator - Performance is slow
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#uzebox)
* Properly update ArkOS version boot text screen

## v1.5 (01/17/2021)
* Updated 64 bit libSDL2 2.10 to libSDL2 2.0.14.1 to fix some tearing (Thanks to Johnny on Flame for suggestion and kreal for compilation)
* Increase audio period and buffer sizes temporarily when running N64 (may improve performance in some games)
* Increase audio period and buffer sizes temporarily when running PSP (may improve performance in some games)

## v1.5 (01/18/2021)
* Fixed retroarch N64 no sound issue from last update

## v1.5 (01/21/2021)
* Adjusted sound configuration in ArkOS so future updates should not impact emulators and ports needing direct access to set sound
* Added correct kyra.dat file to Standalone ScummVM

## v1.5 (01/21/2021-1)
* Fixed deadzone for lzdoom
* Fixed deadzone for Half-Life

## v1.5 (01/24/2021)
* Updated Emulationstation to fix scraping for daphne, neogeo cd, and xegs
* Fixed sound for ppsspp-go emulator
* Added sraping support for tic-80 and sharp x1
* Added official support for Sega Saturn (Performance is slow)
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#sega-saturn)
* Updated battery led script to turn power led red when below 20% and blink red every 1 second when battery life is below 10%

## v1.5 (01/28/2021)
* Updated Drastic to newer 64 bit build (Thanks to slaminger for working with drastic team on getting the fix)
* Updated dosbox_pure core to version 0.10
* Added Crocods (Amstrad CPC) emulator and made it the default emulator for Amstrad CPC (Thanks to JCORR76 for suggeston and testing)
* Added gpsp as a selectable gba core in Emulationstation
* Added 2048 port to ports section
* Added OpenBOR port as system (Thanks to luali for rg351p gamepad workaround)
  * for pak loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#openbor)
  * To exit the emulator, hit the Start button then select exit in the menu for most paks or hit Select+Start
* Added scan script for scummvm games (Thanks to kreal for initial script)
* Set standalone scummvm as default scummvm emulator
* Disabled DSP for Flycast emulator to improve performance for Dreamcast games (Thanks to Bignella for suggestion)
* Added support for Commodore 16
* Added support for Commodore 128
* Updated nes-box theme (Thanks to Jetup)

## v1.5 (01/29/2021)
* Added platform name for scummvm
* Fixed scummvm scan games script to allow for spaces in directory name (Thanks to kreal for fix)
* Added workaround for OpenBor sleep issue
* Fixed loading of scummvm games in retroarch (Thanks to southoz for suggested fix)
* Recompiled dosbox_pure 0.10 core to improve performance (Thanks to Stino for updated Makefile)

## v1.5 (02/03/2021)
* Added TI-99 emulator
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#ti-99)
  * for key configuration, see the global events TI99 Standalone emulator section in the FAQ (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-what-are-the-global-event-keys-and-emulator-event-keys-in-arkos)
  * To exit the emulator, hit Select+Start
* Added retroarch core options reset to default script in Options/Advanced section
* Updated Emulationstation to support ti99 scraping
* Updated TI99 system and background images for nes-box theme (Thanks to Jetup)
* Added support for .hdf extension for Amiga

## v1.5 (02/13/2021)
* Added Flycast32_Rumble core as a selectable core for Atomiswave, Dreamcast and Naomi emulation (Thanks to slaminger for the advice on the core)
* Recompiled scummvm standalone to allow the use of virtual keyboards
* Fixed ability to load .adf for Amiberry (Amiga)
* Updated 32bit and 64bit libgo2 libraries
* Reduced cpu usage of global events hotkey daemon
* Added tools folder into roms partition (Thanks to TadMSTR for suggestion)
  *Allows the ability to add your own tools/scripts. AnberThemes(https://github.com/TadMSTR/AnberThemes) being one such tool.

## v1.5 (02/13/2021-1)
* Added ability to mount and unmount a USB drive from the options menu
  * See FAQ #23 for information on how to use this (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-how-do-i-mount-a-usb-drive-for-copying-and-moving-files).

## v1.5 (02/19/2021)
* Added support for ZX81 emulation (EightyOne libretro core) (Thanks to slaminger for rom testing help)
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#zx81)
* Cleaned up and corrected USB mount script (Thanks to kreal for cleaned up script and Bignella for note on script text mistake)
* Added Pico-8 as a System (roms/pico-8).  
  * for rom loading, see emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#pico-8)
* Updated Emulationstation-fcamod to add scraping for Pico-8 via screenscraper.fr. (Thanks to choo t and kreal for most of the heavy lifting on this.)
* Updated NES box theme to include pico-8 (Thanks to Jetup13)

## v1.5 (02/20/2021)
* Added support for splore and different aspect ratios for Pico-8 (Thanks to onionsaregross and choo t for suggestions)
  * See updated rom loading info in emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#pico-8)

## v1.5 (02/27/2021)
* Added support for Emulationstation Fullscreen
  * Can be switched to from the Options/Advanced section. (ES FullScreen)
  * Can be switched back to the original from the Options/Advanced section. (ES Header)
* Added Retrorun and Retrorun32 emulators for Atomiswave, Dreamcast, Naomi and Saturn (Thanks to luali for the rg351 workaround)
* Added LowRes NX system emulator
* Added Genesis Plus GX Wide 32bit core
* Updated NESBOX theme to add support for fullscreen toggle and LowRes NX(Thanks to Jetup)
* Updated Dosbox-pure to version 0.11
* Fixed scraping for Super Gameboy
* Added support for .dosz files for DOS games

## v1.6 (03/08/2021)
* Updated the kernel and libmali for opengl fixes
* Added easyrpg as ES system
* Updated Emulationstation to support scraping easyrpg
* Fixed retroarch folder ownership
* Fixed samba name and path for the /home/ark folder
* Updated retroarch and retroarch32 core_updater location to new central repository (https://raw.githubusercontent.com/christianhaitian/retroarch-cores/master/aarch64/ and https://raw.githubusercontent.com/christianhaitian/retroarch-cores/master/arm7hf/)
* Updated retroarch and retroarch32 executables to support a more universal screen size for future device support
* Revert lr-MGBA and lr-MGBA_Rumble to 0.8.3 417eb53e commit for best performance (Thanks to Artemis-Ophiel for reporting and testing)
  * Cores have been locked so they can not be accidentally updated through retroarch core updater.  Can be updated by unlocking them in retroarch then doing an update.
* Updated NES-Box theme to support easyrpg
* Added support for ascii art again under Options/Advanced 
  * Included a default loading.ascii file in launchimages roms folder
  * Simply go to Options/Advanced and select Switch launchimage to ascii
  * To switch back to jpg images, simply go to Options and select Switch launchimage to jpg

## v1.6 (03/18/2021)
* Readd support for Tp-Link T2U Nano wifi adapter
* Add sleep 1 to Change Password, Check Current Max Speed, Network Info, Update, and Wifi scripts to decrease occurrence of no control on launch.
* Updated retrorun and retrorun32 with better performance for Sega Dreamcast and slightly better performance for Sega Saturn. (Thanks to valadaa48 for guidance. Thanks to Firebird_WS6, Bignella, and thegreatcrippler for testing and feedback.)
  * For Sega Dreamcast, Retrorun32 and flycast32_rumble core seems to have the overall best performance.
  * For Sega Saturn, Retrorun32 and Yabasanshiro core has the best performance.  Not great but performance has improved.
* Updated global hotkeys system event to use ogage for much less system resource usage.  (Thanks to Valadaa48 for the source and guidance on this.)

## v1.6 (03/18/2021-1)
* Fixed retrorun and retrorun32 coin and button mapping issues for Atomiswave and Naomi
  * L3+A = Pause emulation
  * L3+B = Fast Forward emulation
  * Select + Start = Stop and exit emulation

## v1.6 (04/03/2021)
* Replaced retroarch 64 bit glupen64 core with Mupen64plus 64 bit core (Thanks to Arzeon for recommendation on this)
* Updated perfmax script to only force max speed for emulators that need it such as PSP, N64, and Dreamcast
* Updated ogage service to account for perfmax script change
* Updated retroarches to 1.9.1 (See https://www.libretro.com/index.php/retroarch-1-9-1-released/ for what's new and related changelog)
* Updated hypseus (Daphne Emulator) to version 1.3.0
* Added nice -19 for emulation priority

## v1.6 (04/16/2021)
* Updated ScummVM with AGS support
* Updated DevilutionX to resolve mouse control issue
* Updated Enable Remote Services script to show assigned IP and 5s pause
* Updated perfmax and perfnorm for image blinking fix
* Updated emulationstaton fullscreen and header to not use Batocera's scraping ID
* Updated video shader delay settings

## v1.6 (04/22/2021)
* Added video player
 - See FAQ in wiki for more information and how to use it. (https://github.com/christianhaitian/arkos/wiki/Frequently-Asked-Questions---RG351P#q-how-does-the-movievideo-player-work)
* Added ability to restore retroarch and retroarch32 to default configurations.
* Added UAE4arm_libretro.so for retroarch32 for Amiga and Amiga32 (Thanks to slaminger for the core build)
* Added potator core for Watara Supervision
* Added section for MD MSU (genesis_plus_gx)
* Added ability to restore default retroarch.cfg for both retroarch and retroarch32 from the Options/Advanced menu
* Updated emulationstation to support scraping for Watara Supervision

## vFinal (05/01/2021)
* Added support for the Sonic 1, 2, and CD Ports.
  * See updated ports loading info in emulators and ports section (https://github.com/christianhaitian/arkos/wiki/ArkOS-Emulators-and-Ports-information#sonic-1-rg351pm-and-rg351v-only--coming-soon-to-the-rgb10-rk2020-and-oga-1011)

## vFinal (05/01/2021)
* Fixed Sonic CD exit hotkey daemon
* Resized screens for Sonic 1, 2, and CD to be full screen (Thanks to sonhoon for suggestion)

</br>

# Changelog (wuMMLe)
## (after christianhaitian final update)
</br>

## June 15, 2021
* Update RetroArch to 1.9.6
* Add GX4000

## August 9, 2021
* Street of Rage Remake
* EasyRPG

## September 5, 2021
* Update RetroArch to 1.9.8
* Correct permissions

## September 6, 2021
* Add missing cue extension for Playstation
* Add files for EasyRPG
* Add liblcf, libWildMidi, and libxmp

## October 21, 2021
* Update RetroArch to 1.9.11
* Update EmulationStation
* Add Channel F libretro
* MESS libretro
* QuickNES libretro
* Astrocade
* Satellaview
* Add Astrocade and Channel F to nes-box theme
* Update ThemeMaster

## October 26, 2021
* RetroArch 1.9.11 update to (hopefully) fix missing assets error

## November 17, 2021
* Update RetroArch to 1.9.13
* Update EmulationStation
* Update PPSSPP

## January 13, 2022
* Update RetroArch to 1.9.14
* Add np2kai libretro
* Add sameduck libretro
* Add 32-Bit GPSP GBA libretro core
* Add directories for megaduck and neshacks

## January 14, 2022
* Set GX4000 to use retroarch 1.9.6 due to performance issues
* Add megaduck to nes-box theme

## February 14, 2022
* Update RetroArch
* Add snes9x2005 libretro
* Add pcsx_rearmed_peops libretro (32-bit)
* Add 351Files file browser

## May 14, 2022
* Update exFAT driver from exfat_fuse to exfat_linux
* Update RetroArch

## June 6, 2022
* Update SDL2 to 2.0.18.2
* Add libSDL2_gfx

## October 2, 2022
* Update retroarch info files to make save states work on rumble cores

## December 2, 2022
* Add GZDoom
* Add libzmusic for GZDoom
* Fix ECWolf screen resolution
* Add gptokeyb to system quitter directory
* Install PortMaster v6.58

## December 9, 2022
* Update PPSSPP to 1.13.2

## December 10, 2022
* Update RetroArch to 1.13.0

## December 20, 2022
* Update PPSSPP to 1.14
* Update RetroArch to 1.14.0
* Fix Playstation file extension typo (Credit to K-tec-UK)

## February 2, 2023
* Update PPSSPP to 1.14.4

## March 26, 2023
* Update SDL2 to 2.0.26.2
* Update RetroArch to 1.15.0
* Add swanstation PSX libretro core
* Update mupen64plus
* Update to fix GZDoom for SDL2.0.26.2
* Update scummvm launcher
* Update drastic launcher 
* Update filebrowser (this was later removed from this update because it broke this feature)
* Re-instate PortMaster v6.58

## April 5, 2023
* Revert filebrowser back to working version (if changed from previous update)

## August 25, 2023 
## (The majority of these have been brought in from updates provided by and thanks to christianhaitian and all who contribute!)
* Install and link new SDL 2.0.2800.2 (aka SDL 2.0.28.2)
* Rebuild retroarch v1.15.0 to resolve microstutter issues
* Add retroarch audio and video filters
* Update PPSSPPSDL to v1.15.3-26
* Update ECWolf to 1.4.1 and add mods support
* Add quicknes core for NES and Famicom Disk System
* Add fceumm core to Famicom system
* Add supafaust core for SNES
* Add 32bit gpsp core for GBA
* Add A5200 core as additional core for Atari 5200
* Add puae2021 core for Amiga
* Add Gearsystem and picodrive cores for Sega Master System
* Add Gearsystem core for Game Gear
* Add gearcoleco core for colecovision
* Add fbneo as optional core for NeoGeo CD
* Add coolCV core for colecovision
* Add race core for SNK - NeoGeo Pocket & NeoGeo Pocket Color
* Add Fake08 emulator for PICO-8
* Add Arduboy
* Add vic20 as separate system
* Add microvision
* Updates for Duckstation (PSX)
* Add mame2003_plus to arcade, cps1, cps2, and cps3
* Update cap32 core for Amstrad CPC and GX4000
* Add prg, d71, d81, nib, tap, and vsf support for C64
* Add sgd support for Genesis and MD
* Add chd support for Amiga CD32
* Add .cmd extension support for PC98
* Add cpc and 7z support for Amstrad CPC
* Add 7z support for NeoGeo Pocket and NeoGeo Pocket Color
* Add .mov extension for video player
* Add GLideN64 plugin for mupen64plus standalone
* Add widescreen mode support for mupen64plus-glide64mk2
* Update OpenBOR
* Update NesBox Theme
* Add tool to remove ._ Mac files
* Change mednafen_vb options CPU emulation to fast (VirtualBoy)
* Enable Threaded DSP for 3DO by default
* Default mgba libretro emulator governor to performance
* Force the use of older SDL2 for hypseus due to audio sync issue

## September 2, 2023
* Add Sameboy 0.15.4 for GameBoy
* Add GearBoy for GameBoy
* Update MESS libretro to v0.250
* Set correct display resolution in retroarch config for MESS (critical for Advision)
* Enable option for EmulationStation to Show Last Played
* Update NesBox Theme
* Ensure proper permissions are set on GZDoom, standalone emulators, and libretro cores

## September 7, 2023
* Update EmulationStation

## September 8, 2023
* Update ScummVM to v2.8.0
* Add Sega Pico

## November 5, 2023
* Update Retroarch to v1.16.0
* Update PPSSPP to v1.16.6
* Update flycast and reicast Dreamcast cores
* Fix inability to quit Fake08

## November 22, 2023
* Add thomson
* Add wasm4
* Update NesBox Theme

## December 9, 2023
* Update PortMaster to v8.5.14
* Add script in Advanced Options to fix Start+Select not quitting on RG351P+M

## January 5, 2024
* Update GZDoom and add support for .doom files
* Add fix for asoundrc (add /dev/asound.conf) and
* Add script in Advanced Options to repair asoundrc

## January 29, 2024
* Install psmisc to add killall command for updated gptokeyb

## February 26, 2024
* Fix inability to change controls in gzdoom and lzdoom

## March 20, 2024
* Update RetroArch to 1.17.0
* Update PPSSPP to 1.17.1
* Critical PortMaster update to v2024.03.20-1013
* Add additional RetroArch Filters
* Add Palm mu_libretro core
* Update 64-Bit uae4arm_libretro
* Add stark_shaders for Scummvm and files for Scummvm libretro
* Add XRoar Tandy coco emu
* Add Watara SuperVision
* Add videopac
* Add and fix file extensions for various systems
* Set perfmax to GOVERNOR
* Updated USB DAC control script
* Update NES-Box

## March 21, 2024
* Update gbz35_mod theme

## March 23, 2024
* Add Apple II standalone emulators linapple and shamusworld

## March 28, 2024
* Add AppleWin for Linux Apple II emulator with help from christian_haitian

## March 29, 2024
* Add hatarib_libretro core and set as default core for Atari ST
* Update apple2 script to default detection of linapple conf files in apple2/conf folder when using an .apple2 file

## March 30, 2024
* Update RetroArch to v1.18.0
* Update apple2 script
* Add DoubleCherryGB core for gameboy
* Add stella core for Atari 2600
* Add geolith core and .neo extension for Neo Geo
* Update XRoar to 1.5.5 (Tandy CoCO)

## June 19, 2024
* Update SDL2 to 2.30.3
* RetroArch v1.18.0 update 2
* Update amiga to allow custom config with .user extension and launch amiberry rom-less with .standalone extension
* Add script in tools to select SDL2 version used for Ports
* Update PortMaster if older than 05-14-2024 stable (2024.05.14-XXXX)
* Add aarch64 libzip.so.4
* Add aarch64 libvpx.so.5
* Add aarch64 libiconv.so.2

## July 5, 2024
* Update and fix Change Ports SDL script specifically to accommodate ArkOS on RG351P and RG351M

## September 8, 2024
* Install and Update Python and Python utilities
* Install dos2unix

## November 5, 2024
* Update SDL2 to 2.30.7
* Update RetroArch v1.19.1
* Update xroar Tandy CoCo emulator
* Update script in tools to select SDL2 ver
* Update PortMaster if older than 11-05-2024 stable (2024.11.05-XXXX)

## November 6, 2024
* Set RetroArch screenshots to save in content directory

## November 7, 2024
* Fix mounting method and permissions for exFAT partition in fstab

## December 3, 2024
* Update system OSK

## January 25, 2025
* Update SDL to 2.30.10
* Update GZDoom to 4.13.1
* Update PPSSPP to 1.18.1
* Update XRoar to 1.7.1
* Update Change Ports SDL tool
* Add j2me libretro

## February 20, 2025
* Update RetroArch to v1.20.0
* Update EmulationStation to v2.13.0
* Update GZDoom to 4.14.0 (also fixes strange behavior from previous update)
* Add BBC Micro
* Add .VERSION and .DEVICE files for PortMaster
* Replace supposedly bad freej2me-lr.jar and freej2me-plus-lr.jar files
* Update nes-box and sagabox themes
* Ensure proper file and folder permissions are set

## May 24, 2025
* Update GZDoom to 4.14.2 with fixes thanks to @Jeod and all who contributed (PortMaster)
* Ensure proper file and folder permissions are set
* Transfer contents and remove roms2 folder from root if present (single memory card device does not read from roms2)
