# OpenSimWeather

In-world weather region module for OpenSimulator. Adds configurable weather
states (Clear, Sunny, Rain, Storm, Snow) with viewer-visible particle effects,
optional storm lightning/thunder, environment (windlight) adjustment and wind
integration.

This module was adapted from the `WeatherModule` originally published in the
`GuntharDeNiro/opensim` fork. It is a self-contained `INonSharedRegionModule`
and only depends on standard OpenSim region framework APIs.

## Building

The module is built as part of the OpenSim solution. Its project is discovered
automatically through `addon-modules/*/prebuild.xml` and is also registered in
`OpenSim.sln`.

## Configuration

Copy the settings from `config/OpenSimWeather.ini.example` into your
`OpenSim.ini` (or a region config) and set `Enabled = true` under the
`[Weather]` section.

Once enabled, weather can be controlled in-world over the configured chat
command channel, or it can auto-cycle through presets.
