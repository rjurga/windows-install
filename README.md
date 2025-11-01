# Windows 11 install

## Windows configuration

* Disable automatic updates
  * Edit group policy > Computer Configuration > Administrative Templates > Windows Components > Windows Update > Manage end user experience > Configure Automatic Updates > Disabled
* Disable Bing search in start menu
  * Edit group policy > User Configuration -> Administrative Templates -> Windows Components -> File Explorer -> Turn off display of recent search entries in the File Explorer search box > Enabled
* Disable fast boot and sleep
  * Control Panel > System and Security > Power Options > Choose what the power buttons do
* Disable sleep timeout
  * Settings > System > Power > Screen, sleep, & hibernate timeouts > Make my device sleep after > Never
* Remove unused audio devices
  * Settings > System > Sound > All sound devices > Select device > Audio > Don't allow
* Disable mouse acceleration
  * Settings > Bluetooth & devices > Mouse > Enhance pointer precision > Off
* Always show scrollbars
  * Settings > Accessibility > Visual effects > Always show scrollbars > On
* Disable animation effects
  * Settings > Accessibility > Visual effects > Animation effects > Off
* Disable accessibility keyboard shortcuts
  * Settings > Accessibility > Keyboard > Sticky keys > Keyboard shortcut for Sticky keys > Off
  * Settings > Accessibility > Keyboard > Filter keys > Keyboard shortcut for Filter keys > Off
* Set time to UTC
  * regedit > `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\TimeZoneInformation` > add DWORD value `RealTimeIsUniversal` with hexadecimal value `1`
* Disable indexing
  * Services > Windows Search > Properties > Startup type > Disabled
* Revert to old right click menu in File Explorer
  * regedit > `HKEY_CURRENT_USER\Software\Classes\CLSID` > right click > New > Key > `{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}` > right click > New > Key > `InprocServer32` > (Default) > Value data > empty > OK
* Uninstall useless default apps
* Run windows update

* Set `XDG_CONFIG_HOME` environment variable
  * Edit the system environment variables > Environment Variables > User variables > New > `XDG_CONFIG_HOME` > `%LOCALAPPDATA%`

## Essential software

* [Firefox](https://www.mozilla.org/en-US/firefox/new/)
* [Google Chrome](https://www.google.com/chrome/)
* GPU drivers
  * [AMD](https://www.amd.com/en/support)
  * [Nvidia](https://www.nvidia.com/download/index.aspx)
* [7-Zip](https://www.7-zip.org/)
* [Everything](https://www.voidtools.com/)
* [CPU-Z](https://www.cpuid.com/softwares/cpu-z.html)
* [HWMonitor](https://www.cpuid.com/softwares/hwmonitor.html)
* [System Informer](https://systeminformer.sourceforge.io/)
* [Sumatra PDF](https://www.sumatrapdfreader.org/)

## Development software

* [Hack](https://sourcefoundry.org/hack/)
* [Clink](https://mridgers.github.io/clink/)
* [Git](https://gitforwindows.org/)
* [Fork](https://git-fork.com/)
* [LLVM](https://releases.llvm.org/)
* [CMake](https://cmake.org)
* [Slang](https://shader-slang.com/)
* [Neovim](https://neovim.io/)
  * [Neovide](https://neovide.dev/)
    * Add to right click context menu with the command `:NeovideRegisterRightClick`
  * [vim-plug](https://github.com/junegunn/vim-plug)
    * Copy `plug.vim` to `~/AppData/Local/nvim-data/site/autoload/plug.vim`
  * [ripgrep](https://github.com/BurntSushi/ripgrep)
* [Visual Studio](https://visualstudio.microsoft.com/)
* [RAD Debugger](https://github.com/EpicGamesExt/raddebugger)
* [Python](https://www.python.org/)
* [Visual Studio Code](https://code.visualstudio.com/)
* Graphics Tools
  * Settings > Apps > Optional features > Add an optional feature > Graphics Tools
* [RenderDoc](https://renderdoc.org/)
* [WinMerge](https://winmerge.org/)

## Multimedia software

* [IrfanView](https://www.irfanview.com/)
* [Paint.NET](https://getpaint.net/)
* [mpv](https://mpv.io/)
* [yt-dlp](https://github.com/yt-dlp/yt-dlp)
* [OBS](https://obsproject.com/)
* [foobar2000](https://www.foobar2000.org/)
* [Spotify](https://open.spotify.com/)
* [Steam](https://store.steampowered.com/)
* [Epic Games](https://store.epicgames.com/)

## Misc software

* [Discord](https://discord.com/)
* [WireGuard](https://www.wireguard.com/)
* [qBittorrent](https://www.qbittorrent.org/)
