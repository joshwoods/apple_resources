

- Bundle Resources
- Information Property List
-  SKIncludeConsumableInAppPurchaseHistory 

Property List Key

# SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

## Details 

Type  

boolean

## Discussion

By default, this value is `false`. When it’s `false`, StoreKit doesn’t return finished consumables (unless refunded or revoked) in the transaction information from the following APIs:

- The all sequence in Transaction, which returns the customer’s transaction history for your app

- The latest(for:) in Transaction, which returns the customer’s most recent transaction for a specific product

- The latestTransaction in Product, which provides the customer’s most recent transaction for the product

When you set this value to `true`, StoreKit includes all In-App Purchase transactions — including all finished consumables — in the transaction information when you use the all, latest(for:), and latestTransaction APIs.

Warning

Before you set SKIncludeConsumableInAppPurchaseHistory to `true`, be sure you have a way to reconcile a customer’s consumable transactions on your server, not only on the device. For example, store a transaction’s unique transaction identifier, id, along with its finish state to avoid unintentionally delivering content multiple times if the customer reinstalls the app. Use unfinished to get and process unfinished transactions.

## See Also

### StoreKit

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

