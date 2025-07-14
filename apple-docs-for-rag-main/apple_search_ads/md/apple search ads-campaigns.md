

- Apple Search Ads
-  Campaigns 

API Collection

# Campaigns

Create and manage Search Ads campaigns.

## Overview

You use campaigns to promote your apps in the App Store. For an app to be eligible for Apple Search Ads in a particular market, it must be available for purchase, download, or preorder in the App Store, and Apple Search Ads must be available in the countries and regions you want to promote to. There may be some restrictions that make your app ineligible for Apple Search Ads advertising in some markets. Use Find App Eligibility Records to determine your app eligibility to run in campaigns.

You must have an `adamId` for each app you’re promoting, a valid email address, and an Apple ID. Apple IDs that only use phone numbers aren’t acceptable. All advertisers must comply with Apple Search Ads Advertising Content Policies.

## Topics

### Campaign Endpoints

Create a Campaign

Creates a campaign to promote an app.

Find Campaigns

Fetches campaigns with selector operators.

Get a Campaign

Fetches a specific campaign by campaign identifier.

Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Update a Campaign

Updates a campaign with a campaign identifier.

Delete a Campaign

Deletes a specific campaign by campaign identifier.

### Campaign Request and Response Objects

object Campaign

The response to a request to create and fetch campaigns.

object CampaignResponse

A container for the campaign response body.

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

object CampaignListResponse

The response details of campaign requests.

object CampaignUpdate

The list of campaign fields that are updatable.

object UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

### Data Types

type AdChannelType

The channel type of an ad in a campaign.

type BillingEventType

The type of billing event for a campaign.

type CampaignCountryOrRegionsServingStateReasons

Reasons that displays when a campaign can’t run.

type CampaignDisplayStatus

The status of the campaign.

type CampaignServingStateReasons

Reasons the system provides when a campaign can’t run.

type CampaignServingStatus

The status of the campaign.

type CampaignStatus

The status of the campaign.

type PaymentModel

The payment model that you set.

type SupplySource

The ad placements for a campaign.

## See Also

### Campaigns

Budget Orders

Manage your payment model.

Ad Groups

Create and manage ad groups.

Targeting Keywords and Negative Keywords

Apply relevant words or phrases that make your campaigns findable.

Search Geolocations

Search for apps and geocriteria for your campaigns.

