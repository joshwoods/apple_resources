

- Apple Search Ads
-  Apple Search Ads Campaign Management API 4 

Article

# Apple Search Ads Campaign Management API 4

Learn about changes to Apple Search Ads Campaign Management API 4.

## Overview

API 4 calls are able to access resources created with Apple Search Ads Campaign Management API 5.

### 4.11

Released in April, 2024.

- Added guidance for suggested keyword bid amount to help you increase the likelihood of your ad showing in the App Store. See KeywordBidRecommendation for a summary of changes to Get Keyword-Level Reports.

- You can now create and update budget orders through the API. Added two endpoints: Create a Budget Order and Update a Budget Order. See Budget Orders.

### 4.10

Released in November, 2023.

- Added an endpoint to provide app eligibility according to available supply sources, device classes, age criteria, and countries or regions. See Find App Eligibility Records.

- The Find Targeting Keywords in a Campaign endpoint now supports filtering and sorting by `modificationTime` and `creationTime`.

### 4.9

Released in July, 2023.

Updates to SupplySource:

- Campaigns with a Today tab `SupplySource` no longer serve impressions to iPad.

- Removed minimum asset requirements.

Updates to the ProductPageReason object:

- Updated ad creative rejection reasons.

- Added a ReasonLevel to support the ad approval process.

Important

With the 4.9 release, all previously rejected Today tab ad creatives were `PAUSED` and resubmitted for re-review. The status was updated to `ENABLED` after the re-review. For more information about updating an ad status, see Update an Ad.

### 4.8

Released in April, 2023.

- Added endpoints to support the ad creative approval process for campaigns using the `APPSTORE_TODAY_TAB` or `APPSTORE_SEARCH_RESULTS` SupplySource.

- Find Ad Creative Rejection Reasons and Get Ad Creative Rejection Reasons can help you resolve a ProductPageReason for rejected ad creatives based on Custom Product Pages.

- Find App Assets returns your app asset metadata that may need adjusting.

### 4.7

Released in January, 2023.

- Added Impression Share Reports.

### 4.6.1

Released in October, 2022.

- Added a new section on Rate Limits.

- Updated the script for Create a Client Secret in the OAuth procedures.

- Added a new Find Ad Groups (org-level) endpoint to find ad groups within your organization.

- Added a new Find Ads (org-level) endpoint to find `ads` within your organization.

### 4.6

Released in September, 2022.

Advertisers can book ads using two new ad placements: `APPSTORE_TODAY_TAB` and `APPSTORE_PRODUCT_PAGES_BROWSE`. See SupplySource.

- `APPSTORE_TODAY_TAB` requires an approved ad creative based on eligible Custom Product Pages (CPPs).

- Your CPP needs to be in the `defaultLanguage` of your campaign. See SupplySource.

- The default languages of Hong Kong (HK) and Macau (MO) have been updated from `yue-Hant` to `zh-Hant`. Use the Get Supported Countries or Regions endpoint to fetch supported languages and language codes.

- `APPSTORE_PRODUCT_PAGES_BROWSE` places your ad at the top of the You Might Also Like list when users scroll to the bottom of relevant pages across the App Store.

- An optional app categories targeting dimension is eligible to use with `APPSTORE_PRODUCT_PAGES_BROWSE`. See AppCategoryCriteria.

### 4.4

Released in June, 2022.

- Advertisers are able to book campaigns with a cost-per-tap (`CPC`) pricing model and the `APPSTORE_SEARCH_TAB` SupplySource.

- The cost-per-thousand-impressions (`CPM`) PricingModel has been deprecated. You can’t update a `CPM` campaign to a CPC campaign. You must create new campaigns using `CPC`.

- A lifetime budget is now optional. New campaigns require either a `dailyBudgetAmount` or a `budgetAmount` (lifetime budget), or both. See Create a Campaign and Update a Campaign for payload examples.

- Campaign `endTime` and `startTime` attributes are now configurable. See the Campaign object for validations.

### 4.3

Released in April, 2022.

- Added delete keywords endpoints. See Delete Targeting Keywords and Find Targeting Keywords in a Campaign.

- Enhancements to the geolocation search service.

### 4.2

Released in March, 2022.

- Added `creationTime` field to the Creative, Ad object, AdCreate, AdUpdate, ReportingAd, and `ReportingCreativeSet`.

- Reports now include Get Keyword-Level within Ad Group Reports and Get Search Term-Level within Ad Group Reports.

### 4.1

Released in January, 2022.

Custom Product Pages replaces Creative Sets functionality. The Apple Search Ads API no longer supports Creative Sets and `AdGroupCreativeSets`. Creative Sets APIs return `200 OK` responses with an invalid state. Your Creative Sets data remains available through `Get Creative Set-Level Reports`.

Custom Product Pages reports now include Get Ad-Level Reports, available for campaigns using the `APPSTORE_SEARCH_RESULTS` SupplySource.

### 4.0

Released in May, 2021. You can use calls from the 4.x API to access all of your resources that you created in Apple Search Ads Campaign Management API 3.

#### OAuth

Beginning in 2021, the Apple Search Ads Campaign Management API uses OAuth 2 for API account authentication. Apple Search Ads users no longer use API certificates to manage access to their Search Ads accounts. For more information, see Implementing OAuth for the Apple Search Ads API.

To make calls to the Apple Search Ads Campaign Management API with OAuth, see Calling the Apple Search Ads API.

#### Access Control Lists

Access control lists have the following updates:

- The `parentOrgId` field is a new field in the UserAcl object. This distinguishes the account from an `orgId` belonging to a suborganization. See Calling the Apple Search Ads API for details.

- The Get Me Details endpoint has been added with its MeDetailResponse object.

- The `certExpirationDate` field is no longer a property of the `UserAcl` object.

#### Ad Groups

The `defaultCpcBid` field in the AdGroup object has been renamed to `defaultBidAmount`.

#### Reports

Campaign objects now include new fields: SupplySource, AdChannelType, and BillingEventType. The AdGroup object now includes a new field: PricingModel. Note, in the AdGroup object, the `defaultCpcBid` field used in API 3 is now the `defaultBidAmount` field in API 4.

- Get Campaign-Level Reports returns `supplySources`, AdChannelType, `BillingEventType`, and `avgCPM` in the metadata.

- Get Ad Group-Level Reports returns `PricingModel`, `defaultBidAmount`, and `avgCPM` in the metadata.

- Get Keyword-Level Reports, Get Search Term-Level Reports, and `Get Creative Set-Level Reports` aren’t supported with `supplySources` and AdChannelType fields.

## See Also

### Changelog

Apple Search Ads Campaign Management API 5

Learn about changes to Apple Search Ads Campaign Management API 5.

Apple Search Ads Campaign Management API 3

Apple no longer supports this API.

Apple Search Ads Campaign Management API 2

Apple no longer supports this API.

Apple Search Ads Campaign Management API 1

Apple no longer supports this API.

