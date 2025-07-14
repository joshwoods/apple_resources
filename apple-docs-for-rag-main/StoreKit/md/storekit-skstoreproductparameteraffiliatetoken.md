

- StoreKit
-  SKStoreProductParameterAffiliateToken 

Global Variable

# SKStoreProductParameterAffiliateToken

The key representing the affiliate identifier you wish to use for any purchase made through the view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 11.0+

``` source
let SKStoreProductParameterAffiliateToken: String
```

## Discussion

The value for this key is an instance of NSString.

You receive an affiliate identifier when you sign up for the Affiliate Program. The affiliate associated with this view controller is paid a commission for any items purchased using the controller.

Learn more about the Affiliate Program at https://apple.com/itunes/affiliates.

## See Also

### Affiliate and Analytics Keys

let SKStoreProductParameterProductIdentifier: String

The key representing the product identifier for the promoted product you want the store to display at the top of the page.

let SKStoreProductParameterAdvertisingPartnerToken: String

The key representing the advertising partner you wish to use for any purchase made through the view controller.

let SKStoreProductParameterCampaignToken: String

The key representing an App Analytics campaign.

let SKStoreProductParameterProviderToken: String

The key representing the provider token for the developer that created the app specified by the SKStoreProductParameterITunesItemIdentifier key.

let SKStoreProductParameterCustomProductPageIdentifier: String

The key that represents the custom product page identifier you want the store to display when you present the view controller.

