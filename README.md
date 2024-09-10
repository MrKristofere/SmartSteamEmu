# SmartSteamEmu
Description:
This is a steam client emulator which enables you to play steam games without STEAM client and play online games or lobby enabled-games on LAN without any internet connection or online.

This emulator initially intended only for Age of Empires II HD to enable lobby features without depending on STEAM. Now the emulator has been updated and can be used with other steam's game.

Изображение

Изображение

Изображение

Features:
- Run steam game without steam
- Enables play online OR on LAN without internet connection
- Emulates lobby, server browser
- Stats, Achievements and Save games
- Configurable DLC subscription
- Avatar support
- Plugins support
- Overlay support (DX9/11/OpenGL)
- Steam Workshop partial support

Requirements:
- Microsoft(R) Visual C++ 2010 Runtime (x86)
- .NET Framework 4 (SSELauncher only)
- Steam games

How to use:
- Extract all files to game directory or any directory.
- Open SmartSteamEmu.ini and edit as neccessary.
- Launch SmartSteamLauncher.exe and not the game executable.
- To use different configuration file, add configuration file path
to launcher parameter.

Note:
If you use cracked version that replace steam_api.dll, make sure you restore the original steam_api.dll file first. If your games use CEG or DRM as protection, you might need to regenerate the executables for that computer first (CEG only) or use the cracked version.

Some games may require pre-cracked file to run the games, but be sure steam_api.dll is the original.

Some games such as tomb raider that can host private match require invite friends function to invite others to join their private match. Since this emulator didn't have any invite friend implemented, to JOIN the server press SHIFT+TAB simultaneously.

Beginning with version 1.3.5, online mode is introduced (by SSEOverlay plugin). It will connect to several server (torrent tracker) and STUN server. If you do not wish to connect to these server, it can be disabled completely via overlay settings or modifying its setting file.

Plugin Development:
Plugin is simply a dll file to extend or change the emulator or game behaviour. The dll will be loaded by SmartSteamEmu via LoadLibrary(). Additionally the plugin can have SmartInit() and SmartShutdown() exported function. To get better understanding, download the PDK.

PDK can be downloaded here: viewtopic.php?f=20&t=65200
***************************************************************

Changelog:

Version 1.4.7 (January 18, 2024)
This release focus on Half-Life 25th anniversary update!
- Fix server with password will not be listed as password enabled
- Fix serverbrowser favorite games cannot be removed
- Increase serverbrowser LAN discovery port from 27019 to 27020
- Add S2C_Challenge packet support
- Add fake server filter
- Loader: Add ability to read config file same name as loader (rename loader and .ini to same name)
- Update Steamworks interface to latest one
- NOTE: Most newer interface is stub, so games may not work
- NOTE: Steam Networking is not properly implemented and mostly will not work and may crash
- NOTE: Overlay is not updated
- NOTE: SSELauncher is not updated to reflect new config (Voice enabled by default, voice scale setting, fake filter setting)


Version 1.4.6 (January 11, 2024)
- Finish voice chat implementation, can chat with steam and vice versa
- Add VoiceRecvScale/VoiceSendScale config
- Fix stopping voice chat will causes game to stutter
- Fix server browser where password is not prompted

Version 1.4.5 (January 11, 2024)
- Implement http percentage
- Experiment with voice chat using opus with steam compat

Version 1.4.4 (January 9, 2024)
- Added support for HL 25th Anniversary Edition
- NOTE: There is lot of missing interfaces between this version and last version
- NOTE: Latest interface is not implemented
- NOTE: Compiler has been switched from vs10 to vs14, WinXP is not tested but should work

***************************************************************

Credits:
Thanks to OSW members and supporting friends.
Thanks to all cs.rin.ru Developers Group members including ChrisTX
Thanks to Mitsukarina for helping and maintaining SSELauncher
Thanks to Sisah for helping and maintaining SSEOverlay
Thanks to people who provided translation for SSEOverlay: Czech (Sisah), Russian (Shlak), Spanish (xatornet)
