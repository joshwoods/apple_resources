

- StoreKit
-  SKStoreProductParameterProductIdentifier 

Global Variable

# SKStoreProductParameterProductIdentifier

The key representing the product identifier for the promoted product you want the store to display at the top of the page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 11.0+tvOS 11.0+

``` source
let SKStoreProductParameterProductIdentifier: String
```

## Discussion

The value for this key is an instance of NSString.

When your app uses an SKStoreProductViewController to render an app page for another app, you can optionally choose to highlight an in-app purchase by displaying it at the top of the store page. Set SKStoreProductParameterProductIdentifier to the identifier of the product you want displayed at the top of the page.

The product indicated by the identifier must be set up as a promoted product in the App Store, otherwise the identifier is ignored. See Promoting In-App Purchases.

Note

Use the same product identifiers as used in the productIdentifier variable in the SKProduct class.

## See Also

### Affiliate and Analytics Keys

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

