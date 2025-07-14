

- StoreKit
-  SKStoreProductParameterCampaignToken 

Global Variable

# SKStoreProductParameterCampaignToken

The key representing an App Analytics campaign.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 11.0+

``` source
let SKStoreProductParameterCampaignToken: String
```

## Discussion

The value for this key is an instance of NSString, containing any 40-byte string.

This token allows you to track the effectiveness of your Affiliate Program link and your App Analytics campaign.

For more information about the Affiliate Program, see the Affiliate Program at https://apple.com/itunes/affiliates. For more information about App Store Connect Analytics, see App Store Connect Developer Guide.

## See Also

### Affiliate and Analytics Keys

let SKStoreProductParameterProductIdentifier: String

The key representing the product identifier for the promoted product you want the store to display at the top of the page.

let SKStoreProductParameterAdvertisingPartnerToken: String

The key representing the advertising partner you wish to use for any purchase made through the view controller.

let SKStoreProductParameterAffiliateToken: String

The key representing the affiliate identifier you wish to use for any purchase made through the view controller.

let SKStoreProductParameterProviderToken: String

The key representing the provider token for the developer that created the app specified by the SKStoreProductParameterITunesItemIdentifier key.

let SKStoreProductParameterCustomProductPageIdentifier: String

The key that represents the custom product page identifier you want the store to display when you present the view controller.

