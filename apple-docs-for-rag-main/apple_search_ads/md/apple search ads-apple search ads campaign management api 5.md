

- Apple Search Ads
-  Apple Search Ads Campaign Management API 5 

Article

# Apple Search Ads Campaign Management API 5

Learn about changes to Apple Search Ads Campaign Management API 5.

## Overview

API 5 is the current version.

### 5.2

Released in March, 2025.

- Added endpoints to retrieve app details and localized app details. See Get App Details and Get Localized App Details.

- `APPSTORE_SEARCH_TAB` campaigns require that you Create a Creative using either a default product page or a custom product page as the tap destination. As of API version 5.2, you need to create a default product page ad to use with `APPSTORE_SEARCH_TAB` campaigns. At the release of API version 5.2 Apple automatically creates a default product page ad for all existing, running `APPSTORE_SEARCH_TAB` campaigns.

- The Find App Assets endpoint now supports default product page ads. The Find Ad Creative Rejection Reasons endpoint now supports rejection reasons related to default product pages and product page optimization.

- Added support to use custom product pages as an ad’s tap destination. `APPSTORE_SEARCH_TAB` ad-level metrics are reported through Get Ad-Level Reports. Historical ad-level metrics (before API version 5.2 release) are reported against `adId=-1`. For ad-level metrics after API version 5.2 release, all default product page ads are reported against a new, real `adID` in reporting payloads.

- `APPSTORE_SEARCH_TAB` campaigns can optionally include a deep link. See ProductPageDetail.

### 5.1

Released in October, 2024.

- A read-only `deepLink` field has been added to the ProductPageDetail response. Advertisers can add deep links to custom product pages through App Store Connect. Retrieve your product page metadata with Get Product Pages and Get Product Pages by Identifier endpoints. Deep links are available on iOS 18 and later for Today tab and search results ads, and iPadOS 18 and later for search results ads.

- A correction has been made to the Find Ad Groups endpoint. The selector Condition operator accepts only EQUALS in requests.

### 5.0

Released in May, 2024.

- View-through reporting metrics provide details on Apple Search Ads campaign performance. Installs, new downloads, and redownloads are available as a standalone total, tap-through, and view-through. All reports reflect the new metrics. See SpendRow and ExtendedSpendRow.

- Get Keyword-Level Reports and Get Keyword-Level within Ad Group Reports reflect a new suggestedBidAmount field, replacing deprecated `bidMin` and `bidMax` fields. See KeywordBidRecommendation.

- Get Search Term-Level Reports and Get Search Term-Level within Ad Group Reports require the timezone to be ORTZ.

Other new features include:

- Prior to API 5, new campaigns required a `dailyBudgetAmount` or a `budgetAmount`, or both. A `dailyBudgetAmount` is now a required field for all new campaigns. See Create a campaign.

- Multiple default languages are supported for countries or regions.

Deprecations:

All Creative Sets endpoints are deprecated and unavailable in API 5.

## See Also

### Changelog

Apple Search Ads Campaign Management API 4

Learn about changes to Apple Search Ads Campaign Management API 4.

Apple Search Ads Campaign Management API 3

Apple no longer supports this API.

Apple Search Ads Campaign Management API 2

Apple no longer supports this API.

Apple Search Ads Campaign Management API 1

Apple no longer supports this API.

