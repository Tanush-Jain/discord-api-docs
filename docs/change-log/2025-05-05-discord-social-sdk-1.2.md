---
title: "Discord Social SDK Release 1.2"
date: "2025-05-05"
topics:
  - "Discord Social SDK"
---

A new release of the Discord Social SDK is now available, with the following updates:

### Rich Presence
- Added support for adding custom buttons on activity cards via [`Activity::AddButton`]

### Packaging
- Unity and Unreal plugin artifacts now contain just the additional files for console support so they can be extracted on top of the base plugin
- Unity plugin is now packaged as a .zip that you should extract inside the Packages directory of your project to enable the above
- Console archives now contain a small README with some console-specific documentation

### Misc
- Added [`Client::OpenConnectedGamesSettingsInDiscord`] for deeplinking into Discord's settings for connected games, which provides players some control over who can DM them
- Fixed a hang that could occur on Linux in [`Client::RegisterLaunchCommand`] and [`Client::RegisterLaunchSteamApplication`]
- [`Client::RegisterLaunchCommand`] and [`Client::RegisterLaunchSteamApplication`] now work from inside the Steam Runtime on Linux
- Fixed a crash on exit that could occur when there were pending callbacks in the queue

<!-- Autogenerated Reference Links -->
[`Activity::AddButton`]: https://discord.com/developers/docs/social-sdk/classdiscordpp_1_1Activity.html#aab07650fcff18565eb78a1e2df46627e
[`Client::OpenConnectedGamesSettingsInDiscord`]: https://discord.com/developers/docs/social-sdk/classdiscordpp_1_1Client.html#a24f268f5eebe9919a3f774354eb577e0
[`Client::RegisterLaunchCommand`]: https://discord.com/developers/docs/social-sdk/classdiscordpp_1_1Client.html#a024d7222931fdcb7d09c2b107642ecab
[`Client::RegisterLaunchSteamApplication`]: https://discord.com/developers/docs/social-sdk/classdiscordpp_1_1Client.html#a45b2c791c5b06f77d457dacb53dfba40