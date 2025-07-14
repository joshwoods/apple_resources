

- App Store Connect API
- App Store Connect API Release Notes
-  App Store Connect API 3.2 release notes 

Article

# App Store Connect API 3.2 release notes

Update your server-side code to use new features, and test your code against API changes.

## Overview

App Store Connect API version 3.2 provides resources that enable you to automate actions you take in App Store Connect.

### New Features

- visionOS is now available in multiple endpoints. App Store Connect API now supports `APP_APPLE_VISION_PRO` for ScreenshotDisplayType, and `APPLE_VISION_PRO` for PreviewType.

- A new `Installs` report type is available with four subtypes: `SUMMARY_INSTALL_TYPE, SUMMARY_TERRITORY, SUMMARY_CHANNEL,` and `DETAILED.` For more information see Download Sales and Trends Reports.

- You can now add achievements and leaderboard entries with POST /v1/gameCenterPlayerAchievementSubmissions and POST /v1/gameCenterLeaderboardEntrySubmissions.

- GameCenterMatchmakingQueue now supports backwards compatibility with the addition of a new attribute `classicMatchmakingBundleIds`.

- You can now download Xcode Cloud `Notarized and Stapled App` artifacts through the Public API. For more information, see CiArtifact.Attributes.

- The attribute `baseTerritory` is now required when creating an In App Purchase. For more information, see InAppPurchasePriceScheduleCreateRequest.

### Deprecations

- The enum `availableInAllTerritories` is no longer available for pricing related endpoints. For more information, see InAppPurchasePriceScheduleCreateRequest.

- The player attribute is now removed from GameCenterLeaderboardEntrySubmissionCreateRequest.Data.Attributes.

- The `notarizations` value type is now removed from CiActionType.

## See Also

### Versions

App Store Connect API 3.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.7 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.6 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.5 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.4 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.3 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.1 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.0 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.4 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.3 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.2 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.1 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 2.0 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 1.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 1.7 release notes

Update your server-side code to use new features, and test your code against API changes.

