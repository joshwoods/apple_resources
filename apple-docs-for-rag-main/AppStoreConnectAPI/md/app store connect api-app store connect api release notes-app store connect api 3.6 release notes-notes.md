

- App Store Connect API
- App Store Connect API Release Notes
-  App Store Connect API 3.6 release notes 

Article

# App Store Connect API 3.6 release notes

Update your server-side code to use new features, and test your code against API changes.

## Overview

App Store Connect API version 3.6 provides resources that enable you to automate actions you take in App Store Connect.

### New Features

- Win-back offers can now be configured using Win-back offers. These are offers to bring back churned or expired customers to a subscription. To learn more, see Creating and configuring win-back offers.

- Developers can now use Subscription images and In-app purchase images endpoints to manage images for promoting subscriptions and in-app purchases.

- Age ratings for Australia and Korea can be read using Read App Info Information.

- There are two new attributes available for age rating declarations. Use Modify an Age Rating Declaration to set the attributes `lootbox` and `koreaAgeRatingOverride`, to learn more, see AgeRatingDeclarationUpdateRequest.Data.Attributes.

- The `INSTALLS` report type now has a detailed and summary monthly option for Download Sales and Trends Reports.

- The TerritoryAvailability.Attributes resource now has two additional `contentStatuses` possible values, `ICP_NUMBER_MISSING` and `ICP_NUMBER_INVALID`. To learn more, see the “Availability in China mainland” section in App Store Connect Help.

- Developers can now upload screenshots for Apple Watch Series 10, to learn more about possible values, see ScreenshotDisplayType.

- Developers can now add an app encryption declaration for a given app using Create an app encryption declarations.

### Improvements

- The OpenAPI specification (downloadable here) values has improved `operationId` names and the Apple managed Swift OpenAPI generator now produces more readable names for the App Store Connect API operations.

- SubscriptionStatusUrlVersion normalized to all caps values such as `V1` and `V2`.

- The List Apps resources now has more optional filters, including `reviewSubmissions.state`, `reviewSubmissions.platform`. The optional field `appAvailabilityV2` is also now available.

- The Read App Store Version Information endpoint now includes `gameCenterAppVersions` fields.

- The List All Price Points for a Subscription endpoint now requires a `territory` filter.

- The `purchaseRequirement` attribute for AppEvent.Attributes now correctly shows as a `string` type.

### Deprecations

- The `app` relationship to Create an app encryption declarations has been deprecated.

- The Promoted Purchase Images endpoints have been deprecated and replaced with Subscription images and In-app purchase images.

### Removals

- The duration `ONE_DAY` has been removed from from SubscriptionOfferDuration.

## See Also

### Versions

App Store Connect API 3.8 release notes

Update your server-side code to use new features, and test your code against API changes.

App Store Connect API 3.7 release notes

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

