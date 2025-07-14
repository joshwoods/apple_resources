

- StoreKit
-  Storefront 

Structure

# Storefront

The region and unique identifier of the App Store storefront for the device.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Storefront
```

## Mentioned in 

Testing In-App Purchases with sandbox

## Overview

In-app products you create through App Store Connect are available for sale in each region with an App Store. You can use the storefront information to determine the customer’s region, and offer in-app products suitable for that region.

You need to maintain your own list of product identifiers and the storefronts where you want to make them available.

Note

Don’t save the storefront information with your customer information because storefront information can change at any time. Get the storefront identifier immediately before you display product information or availability in your app. Don’t use storefront information to develop or enhance a customer profile, or to track customers for advertising or marketing purposes.

### Change the App Store country or region in the sandbox environment

When you change the App Store Country or Region in App Store Connect for a Sandbox Apple Account, it changes the storefront in your app. Change the region to test In-App Purchases for different regions in your app. For more information about changing the App Store Country or Region in App Store Connect, see Test in-app purchases.

Important

To successfully activate a storefront after you change the region in App Store Connect, sign out of the Sandbox Apple Account on the device and sign back in.

## Topics

### Identifying the storefront

static var current: Storefront?

The current App Store storefront for product purchases.

let countryCode: String

The three-letter code that represents the country or region associated with the App Store storefront.

let id: String

An Apple-defined value that uniquely identifies an App Store storefront.

### Listening for storefront changes

static var updates: Storefront.Storefronts

The asynchronous sequence that emits storefront information when the system updates the storefront.

struct Storefronts

An asynchronous sequence that listens for changes to the storefront.

### Getting the currency for the storefront

var currency: Locale.Currency?

The currency that the storefront uses.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Storefront information

static var current: Storefront?

The current App Store storefront for product purchases.

static var updates: Storefront.Storefronts

The asynchronous sequence that emits storefront information when the system updates the storefront.

