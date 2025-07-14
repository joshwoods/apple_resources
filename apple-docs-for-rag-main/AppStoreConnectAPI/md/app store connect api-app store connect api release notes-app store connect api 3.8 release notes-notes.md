

- App Store Connect API
- App Store Connect API Release Notes
-  App Store Connect API 3.8 release notes 

Article

# App Store Connect API 3.8 release notes

Update your server-side code to use new features, and test your code against API changes.

## Overview

App Store Connect API version 3.8 provides resources that enable you to automate actions you take in App Store Connect.

### New Features

- The Merchant ID resource is now available to automate tasks related to Apple Pay and Apple Wallet. Apple Pay certificates now have enum values on the `certificates` resource.

- Modify a certificate is now available. Use this endpoint to modify the activation status of your Payment Processing certificate. To learn more, see Managing merchant IDs and Payment Processing certificates.

- Create public links that accept testers with specific device and OS combinations using the `betaRecruitmentCriteria` resource. To learn more, see Beta recruitment criteria.

- Use the new `nominations` resource to share your new content, app enhancement, or app launch with Apple. To learn more see, Getting featured on the App Store.

- Three new content statuses, `TRADER_STATUS_NOT_PROVIDED`, `TRADER_STATUS_VERIFICATION_FAILED`, and `TRADER_STATUS_VERIFICATION_STATUS_MISSING` are available for TerritoryAvailability.Attributes. To learn more, see Manage European Union Digital Services Act trader requirements.

### Improvements

- The field `iosBuildsAvailableForAppleVision` is now in the Beta Groups resource.

### Deprecations

- The attribute `brazilAgeRatings` for AppInfo.Attributes is deprecated. Use `brazilAgeRatingV2` instead.

### Removals

- The `PromotedPurchaseImages` resources is now removed and replaced with Subscription images and In-app purchase images.

- The enum `ELAPSED_TIME_MILLISECOND` is now removed from GameCenterLeaderboardFormatter.

## See Also

### Versions

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

