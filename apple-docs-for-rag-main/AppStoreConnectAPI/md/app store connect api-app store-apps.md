

- App Store Connect API
- App Store
-  Apps 

API Collection

# Apps

Manage your apps in App Store Connect.

## Overview

An `apps` resource represents your app that’s currently in development, or available on the App Store through the App Store Connect website. Use the `apps` resource to manage and maintain your existing apps.

Don’t use this API to create new apps; instead, create new apps on the App Store Connect website. To upload builds to App Store Connect, you must use Xcode, Transporter, or the Transporter Mac app. This API doesn’t permit you to directly upload your builds, but you may use App Store Connect API Keys in conjunction with Transporter to upload. To download the Transporter app, see the Mac App Store.

To learn more about managing your apps, see Add a new app.

## Topics

### Getting and modifying app information

List Apps

Find and list apps in App Store Connect.

Read App Information

Get information about a specific app.

Modify an App

Update app information, including bundle ID, primary locale, price schedule, and global availability.

Read an App’s Encryption Declarations

Find and list all available app encryption declarations.

### Getting app build and prerelease version information

List All Builds of an App

Get a list of builds associated with a specific app.

List All Prerelease Versions for an App

Get a list of prerelease versions associated with a specific app.

### Getting App Clip information

List All App Clips for an App

List your app’s associated App Clips.

### Getting beta tester information for TestFlight

List All Beta Groups for an App

Get a list of beta groups associated with a specific app.

Remove Specified Beta Testers from All Groups and Builds of an App

Remove one or more beta testers’ access to test any builds of a specific app.

### Getting an app’s TestFlight details

Read the Beta App Review Details Resource of an App

Get the beta app review details for a specific app.

Read the Beta License Agreement of an App

Get the beta license agreement for a specific app.

List All Beta App Localizations of an App

Get a list of localized beta test information for a specific app.

### Getting an app’s Xcode Cloud products

Read the Xcode Cloud Product for an App

Get the Xcode Cloud product information for an app you build with Xcode Cloud.

### Getting an app’s price points

List all price points for an app

Get all the available price points for a specific app.

Read app price point information

Get details about a specific app price point.

List app price point equalizations

List all equivalent app prices points to a base price point.

### Getting App Store details for your app

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

GET /v1/apps/{id}/appStoreVersionExperimentsV2

### Getting in-app purchase information

Read In-App Purchase Information

Get information about an in-app purchase.

Deprecated

List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

List All In-App Purchases for an App V1

List the in-app purchases that are available for your app.

Deprecated

### Getting review submissions

Get review submissions for an app

Get a list of review submissions associated with a specific app.

### Getting power and performance metrics

Get Power and Performance Metrics for an App

Get the performance and power metrics data for the most recent version of an app.

### Getting customer reviews

List All Customer Reviews for an App

Get a list of customer reviews for a specific app.

### Getting and managing an app’s price schedules

Read price schedule information for an app

Read price schedule details for a specific app.

Read an app's price schedule information

List the price schedule details for a specific app.

List automatically generated prices for an app

List the automatically calculated prices for an app generated from a base territory.

Read the base territory for an app's price schedule

Read the base territory and currency for a specific app.

List manually chosen prices for an app

List the prices you chose for a specific app.

Add a scheduled price change to an app

Create a scheduled price change for an app.

### Getting and managing an app’s availability

List availability for an app

Get a list of availabilities for a specific app.

### Getting beta tester metrics

Read beta tester metrics for an app

Get usage metrics for beta testers of a specific app.

### Getting alternative distribution information

Read an app’s alternative distribution key

Get the alternative distribution keys for a specific app.

Read the marketplace search detail URL

Get search detail URL for the alternative marketplace.

### Objects and data types

object App

The data structure that represents an Apps resource.

object AppWithoutIncludesResponse

object AppsWithoutIncludesResponse

object AppUpdateRequest

The request body you use to update an App Update.

object AppClipsResponse

A response that contains a list of App Clips resources.

object AppResponse

A response that contains a single Apps resource.

object AppsResponse

A response that contains a list of Apps resources.

object InAppPurchase

The data structure that represents the In-App Purchases resource.

Deprecated

object InAppPurchaseResponse

A response that contains a single In-App Purchases resource.

Deprecated

object InAppPurchasesResponse

A response that contains a list of In-App Purchases resources.

Deprecated

object AppBetaTestersLinkagesRequest

A request body you use to remove beta testers from an app.

object AppPricePointV3

The data structure that represents an App Price Point V3 resource.

object AppPricePointV3Response

object AppPricePointsV3Response

object AppPriceSchedule

object AppPriceScheduleCreateRequest

object AppPriceScheduleResponse

object AppPriceV2

object AppPriceV2InlineCreate

The data structure that represents a App Price V2 Inline Create resource.

object AppPricesV2Response

object TerritoryInlineCreate

type Platform

Strings that represent Apple operating systems.

type SubscriptionStatusUrlVersion

Strings that represent versions of App Store Server Notifications.

object App.Relationships.InAppPurchases

The data and links that describe the relationship between the resources.

Deprecated

## See Also

### Apps and App Metadata

App Metadata

Manage the metadata of apps in App Store Connect.

Custom Product Pages and Localizations

Create and manage your app’s custom product pages and localizations.

App Events and Metadata

Create and schedule in-app events and manage in-app event metadata.

