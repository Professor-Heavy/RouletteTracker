# RouletteTracker

A Dalamud plugin that locally tracks duties from roulettes in _Final Fantasy XIV_.

> [!IMPORTANT]
> The sections beneath are taken from Dalamud's [SamplePlugin repository](https://github.com/goatcorp/SamplePlugin) and are kept for future purposes.

### Building

1. Open up `SamplePlugin.sln` in your C# editor of choice (likely [Visual Studio 2022](https://visualstudio.microsoft.com) or [JetBrains Rider](https://www.jetbrains.com/rider/)).
2. Build the solution. By default, this will build a `Debug` build, but you can switch to `Release` in your IDE.
3. The resulting plugin can be found at `SamplePlugin/bin/x64/Debug/SamplePlugin.dll` (or `Release` if appropriate.)

### Activating in-game

1. Launch the game and use `/xlsettings` in chat or `xlsettings` in the Dalamud Console to open up the Dalamud settings.
    * In here, go to `Experimental`, and add the full path to the `SamplePlugin.dll` to the list of Dev Plugin Locations.
2. Next, use `/xlplugins` (chat) or `xlplugins` (console) to open up the Plugin Installer.
    * In here, go to `Dev Tools > Installed Dev Plugins`, and the `SamplePlugin` should be visible. Enable it.
3. You should now be able to use `/pmycommand` (chat) or `pmycommand` (console)!

Note that you only need to add it to the Dev Plugin Locations once (Step 1); it is preserved afterwards. You can disable, enable, or load your plugin on startup through the Plugin Installer.
