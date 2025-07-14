

- StoreKit
- SKStoreProductViewController
-  Product Dictionary Keys 

API Collection

# Product Dictionary Keys

Keys for identifying products and the tokens for affiliates and campaigns.

## Overview

These dictionary keys are used in the parameter for the loadProduct(withParameters:completionBlock:) method.

The SKStoreProductParameterITunesItemIdentifier key represents the product to display, and is always required. Other keys provide optional affiliate or promoted product information.

Learn more about the Affiliate Program at https://apple.com/itunes/affiliates.

## Topics

### Required Key

let SKStoreProductParameterITunesItemIdentifier: String

The key representing the iTunes identifier for the item you want the store to display when the view controller is presented.

### Affiliate and Analytics Keys

let SKStoreProductParameterProductIdentifier: String

The key representing the product identifier for the promoted product you want the store to display at the top of the page.

let SKStoreProductParameterAdvertisingPartnerToken: String

The key representing the advertising partner you wish to use for any purchase made through the view controller.

let SKStoreProductParameterAffiliateToken: String

The key representing the affiliate identifier you wish to use for any purchase made through the view controller.

let SKStoreProductParameterCampaignToken: String

The key representing an App Analytics campaign.

let SKStoreProductParameterProviderToken: String

The key representing the provider token for the developer that created the app specified by the SKStoreProductParameterITunesItemIdentifier key.

let SKStoreProductParameterCustomProductPageIdentifier: String

The key that represents the custom product page identifier you want the store to display when you present the view controller.

## See Also

### Loading a new product screen

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

func loadProduct(withParameters: [String : Any], completionBlock: ((Bool, (any Error)?) -> Void)?)

Loads a new product screen to display.

func loadProduct(withParameters: [String : Any], impression: SKAdImpression, completionBlock: ((Bool, (any Error)?) -> Void)?)

func loadProduct(parameters: [String : Any], impression: AppImpression) async throws

func loadProduct(parameters: [String : Any], impression: AppImpression, reengagementURL: URL) async throws

