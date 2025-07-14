

- Apple Search Ads
-  Targeting Keywords and Negative Keywords 

API Collection

# Targeting Keywords and Negative Keywords

Apply relevant words or phrases that make your campaigns findable.

## Overview

Ad groups use two keyword object types: `targeting` and `negative`. Use targeting keywords to show ads according to relevant search terms people might use to find your app. Use negative keywords with campaigns and ad groups to prevent ads from showing in App Store searches.

See the Enable and Disable Search Match section of Ad Groups for details about how to automatically show ads for search terms relevant to your app. You can use up to 5000 targeting keywords and negative keywords per ad group, and up to 1000 keywords per API call. Keywords are case-insensitive.

## Topics

### Ad Group Targeting Keywords Endpoints

Create Targeting Keywords

Creates targeting keywords in ad groups.

Find Targeting Keywords in a Campaign

Fetches targeting keywords in a campaign’s ad groups.

Get a Targeting Keyword in an Ad Group

Fetches a specific targeting keyword in an ad group.

Get All Targeting Keywords in an Ad Group

Fetches all targeting keywords in ad groups.

Update Targeting Keywords

Updates targeting keywords in ad groups.

Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

### Campaign Negative Keywords Endpoints

Create Campaign Negative Keywords

Creates negative keywords for a campaign.

Find Campaign Negative Keywords

Fetches negative keywords for campaigns.

Get a Campaign Negative Keyword

Fetches a specific negative keyword in a campaign.

Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

### Ad Group Negative Keywords Endpoints

Create Ad Group Negative Keywords

Creates negative keywords in a specific ad group.

Find Ad Group Negative Keywords

Fetches negative keywords in a campaign’s ad groups.

Get an Ad Group Negative Keyword

Fetches a specific negative keyword in an ad group.

Get All Ad Group Negative Keywords

Fetches all negative keywords in ad groups.

Update Ad Group Negative Keywords

Updates negative keywords in an ad group.

Delete Ad Group Negative Keywords

Deletes negative keywords from an ad group.

### Keywords Request and Response Objects

object Keyword

Targeting keyword parameters to use in requests and responses.

object NegativeKeyword

Negative keyword parameters to use in requests and responses.

object KeywordResponse

A container for the targeting keywords response body.

object KeywordListResponse

The response details of targeting keyword requests.

object KeywordUpdateRequest

Targeting keyword parameters to use in requests and responses.

object NegativeKeywordResponse

A container for the negative keyword response body.

object NegativeKeywordListResponse

The response details of negative keyword requests.

## See Also

### Campaigns

Campaigns

Create and manage Search Ads campaigns.

Budget Orders

Manage your payment model.

Ad Groups

Create and manage ad groups.

Search Geolocations

Search for apps and geocriteria for your campaigns.

