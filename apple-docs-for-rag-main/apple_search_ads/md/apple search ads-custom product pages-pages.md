

- Apple Search Ads
-  Custom Product Pages 

API Collection

# Custom Product Pages

View Custom Product Page details.

## Overview

In iOS 15 and later, you can use custom product pages that you build in App Store Connect to create ad variations in the Apple Search Ads Campaign Management API to promote your apps.

To create a custom product page ad, use the following workflow:

1.  Use Get Product Pages to fetch your `productPageId`.

2.  Use Get Product Page Locales to fetch locale metadata and supported languages. Verify that your custom product page locale and asset data match the language and device types in your campaign AdGroup.

3.  Use Create a Creative with your `productPageId` to obtain a `creativeId`.

4.  Use Create an Ad with a `creativeId` to assign a custom product page to an AdGroup. Each ad group can have one custom product page. For information about how to update a custom product page ad group assignment, see Update an Ad.

5.  Use Get Ad-Level Reports to track the performance of ads in your campaigns. These details help you optimize your Apple Search Ads campaigns to deliver a contextualized customer experience.

Note

If you’ve been using Creative Sets with the API, see section 4.1 in Apple Search Ads Campaign Management API 4 for Creative Sets deprecation details.

## Topics

### Product Page Endpoints

Get Product Pages

Fetches metadata of all your custom product pages.

Get Product Pages by Identifier

Fetches metadata for a specific product page.

Get Product Page Locales

Fetches product page locales by identifier.

Get Supported Countries or Regions

Fetches supported languages and language codes.

Get App Preview Device Sizes

Fetches supported app preview device-size mappings.

### Product Page Request and Response Objects

object LocaleInfo

The supported languages and language codes.

object CountryOrRegion

The supported locales of a product page.

object CountriesOrRegionsListResponse

A container for product page responses.

object MediaAppVideoAsset

The app preview or screenshot asset detail.

object ProductPageLocaleDetail

The product page locale metadata on App Store Connect.

object ProductPageDetail

The product page metadata.

object ProductPageDetailWithAssets

The product page asset metadata.

object ProductPageLocaleDetailListResponse

A container for product page responses.

object ProductPageDetailResponse

A container for product page responses.

object ProductPageDetailWithAssetInfoResponse

A container for product page responses.

object ProductPageDetailListResponse

A container for product page responses.

object ProductPageReasonCreate

The ad creative rejection reason based on a product page.

## See Also

### Custom Product Page Ads

Ads

Assign an ad creative to an ad group.

Ad Rejection Reasons

Review reasons for an ad rejection.

Creatives

Create and manage ad creatives within your organization.

