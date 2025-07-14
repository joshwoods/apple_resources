

- App Store Connect API
- App Store Connect API Release Notes
-  App Store Connect API 3.7 release notes 

Article

# App Store Connect API 3.7 release notes

Update your server-side code to use new features, and test your code against API changes.

## Overview

App Store Connect API version 3.7 provides resources that enable you to automate actions you take in App Store Connect.

### New Features

- Developers now need to provide a description for all beta localizations before submitting to beta app review for external testing with TestFlight. You can update `betaAppLocalizations` with Modify a Beta App Localization.

- Added `WIN_BACK_ELIGIBILITY` report type to Download Sales and Trends Reports.

- Name is now a required field when using Create an App Info Localization. To see other attributes you can create or modify, see AppInfoLocalizationCreateRequest.Data.Attributes.

- Developers can now look up in-app purchase price point equalization using List all in-app purchase price point equalizations.

- The enum `UNIVERSAL` is now added to BundleIdPlatform. To learn more, see Preparing your app for distribution.

- The enums `DEVELOPER_ID_APPLICATION_G2` and `DEVELOPER_ID_KEXT_G2` are now available when using CertificateType. To learn more, see Notarizing macOS software before distribution and macOS Code Signing Tips and Tricks.

- You can now read age ratings for France by using Read App Info Information.

- The Read an app’s alternative distribution key endpoint now shows multiple distribution keys when you have multiple configured.

- There is a new required attribute `defaultFormatter` when you use Create a leaderboard, which gives all your localizations the same formatter. To learn more, see GameCenterLeaderboardCreateRequest.Data.Attributes.

### Deprecations

- The attribute `previewImage` on AppPreview.Attributes is deprecated. Use `previewFrameImage` and PreviewFrameImage instead.

- The attribute `assetDeliveryState` on AppPreview.Attributes is deprecated. Use `videoDeliveryState` and AppMediaVideoState instead.

- The attribute `previewImage` on AppEventVideoClip.Attributes is deprecated. Use `previewFrameImage` and PreviewFrameImage instead.

- The attribute `assetDeliveryState` on AppEventVideoClip.Attributes is deprecated. Use `videoDeliveryState` and AppMediaVideoState instead.

- The attribute `appStoreState` on AppInfo.Attributes is deprecated. Use `state` instead.

- The attribute `appStoreState` on AppStoreVersion.Attributes is deprecated. Use `appVersionState` and AppVersionState instead.

- The relationship `groupLeaderboardSet` on GameCenterLeaderboardSet.Relationships is deprecated.

- The relationship `groupAchievement` on GameCenterAchievement.Relationships is deprecated.

- The relationship `groupLeaderboard` on GameCenterLeaderboard.Relationships is deprecated.

### Removals

- The `v1/appPreOrders` and `v1/appAvailabilities` resources are removed and replaced with `v2/appAvailabilities`. To learn more, see App availability.

- `WATCH_SERIES_4` and `WATCH_SERIES_3` enums are removed from PreviewType.

- The `subscription` include for Read the availability of a subscription is removed.

## See Also

### Versions

App Store Connect API 3.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.6 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.5 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.4 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.3 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.2 release notes

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

