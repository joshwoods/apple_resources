

- Apple Search Ads
-  Ad Groups 

API Collection

# Ad Groups

Create and manage ad groups.

## Overview

An ad group is a collection of criteria that defines who sees your ad in App Store search results. A basic ad group includes a `startTime`, `endTime`, and `dailyBudgetAmount`. You can add bid amounts, TargetingDimensions, and Targeting Keywords and Negative Keywords. Use the Search for Geolocations endpoint to find localities to use for targeting dimensions within ad groups.

### Build a Campaign Keywords Strategy

When building a campaign promotion strategy, you define keywords relevant to your app and bid on them. Relevant keywords increase the viability of your app to rank high in user searches. You can either automate your keyword and bid strategy by using the Search Match feature, or use your own keywords and bid strategy.

The Search Match feature is an algorithm that uses multiple resources to match your ad to relevant searches in the App Store. The resources include metadata from your App Store product page, information about similar apps in the same genre, and other available search data. Search Match is a good option if you don’t want to figure out all keyword possibilities and actively bid on them.

### Enable and Disable Search Match

To enable Search Match, use Create an Ad Group or Update an Ad Group endpoints to perform the following steps:

1.  Set `automatedKeywordsOptIn: true`.

2.  Set the required field `defaultBidAmount`.

If you’re using your own keywords and bid strategy, disable Search Match using Create an Ad Group or Update an Ad Group endpoints using the following steps:

1.  Set `automatedKeywordsOptIn: false`.

2.  Set the required field `defaultBidAmount`.

3.  Use the `bidAmount` field in `Create Targeting Keywords` and `Update Targeting Keywords` endpoints to set a threshold price for a keyword in a bidding auction.

Important

If you don’t provide a `bidAmount`, the `bidAmount` uses the `defaultBidamount` of the corresponding ad group.

## Topics

### Ad Group Endpoints

Create an Ad Group

Creates an ad group as part of a campaign.

Find Ad Groups

Fetches ad groups within a campaign.

Find Ad Groups (org-level)

Fetches ad groups within an organization.

Get an Ad Group

Fetches a specific ad group with a campaign and ad group identifier.

Get all Ad Groups

Fetches all ad groups with a campaign identifier.

Update an Ad Group

Updates an ad group with an ad group identifier.

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

### Ad Group Request and Response Objects

object AdGroup

The response to ad group requests.

object AdGroupUpdate

The response to ad group update requests.

object AdGroupResponse

A container for the ad group response body.

object AdGroupListResponse

The response details of ad group requests.

### Audience Refinement

object TargetingDimensions

The optional criteria to use with ad groups to narrow the audience that views your ads.

object AppCategoryCriteria

The defined target audience by app category.

object AppDownloaderCriteria

The defined targeted audience according to app downloads.

object AdminAreaCriteria

The defined targeted audience by administrative area.

object CountryCriteria

The defined targeted audience by country or region.

object LocalityCriteria

The defined targeted audience by locality.

object AgeCriteria

The defined targeted audience to include using the age demographic.

object AgeRange

The defined target audience to include using the age-range demographic.

object DaypartCriteria

The defined targeted audience to include for a specific time of day.

object DaypartDetail

The defined targeted audience to include by a specific time of day.

object DeviceClassCriteria

The defined targeted audience to include by device type.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

### Data Types

type AdGroupDisplayStatus

The status of the ad group.

type AdGroupServingStateReasons

A list of reasons that displays when an ad group isn’t running.

type AdGroupServingStatus

The status of whether the ad group is serving.

type AdGroupStatus

The status of whether the ad group is enabled or not.

type DeviceClass

The defined targeted audience to include by device type.

type Gender

The defined targeted audience in a campaign.

type PricingModel

The type of pricing model for a bid.

## See Also

### Campaigns

Campaigns

Create and manage Search Ads campaigns.

Budget Orders

Manage your payment model.

Targeting Keywords and Negative Keywords

Apply relevant words or phrases that make your campaigns findable.

Search Geolocations

Search for apps and geocriteria for your campaigns.

