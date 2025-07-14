

- StoreKit
-  SKStoreProductParameterProviderToken 

Global Variable

# SKStoreProductParameterProviderToken

The key representing the provider token for the developer that created the app specified by the SKStoreProductParameterITunesItemIdentifier key.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.0+macOS 11.0+

``` source
let SKStoreProductParameterProviderToken: String
```

## Discussion

The value for this key is an instance of NSString.

Use your own provider token when cross promoting your own apps. This token lets you track the effectiveness of the cross promotion effort separate from any affiliate campaign that shares the same campaign token.

When promoting apps for other developers, use their provider token instead. In this case, the token lets the developer track the effectiveness of your App Analytics campaign for their apps.

The key must be used in combination with your campaign token, SKStoreProductParameterCampaignToken. For more information, see App Store Connect Developer Guide.

## See Also

### Affiliate and Analytics Keys

let SKStoreProductParameterProductIdentifier: String

The key representing the product identifier for the promoted product you want the store to display at the top of the page.

let SKStoreProductParameterAdvertisingPartnerToken: String

The key representing the advertising partner you wish to use for any purchase made through the view controller.

let SKStoreProductParameterAffiliateToken: String

The key representing the affiliate identifier you wish to use for any purchase made through the view controller.

let SKStoreProductParameterCampaignToken: String

The key representing an App Analytics campaign.

let SKStoreProductParameterCustomProductPageIdentifier: String

The key that represents the custom product page identifier you want the store to display when you present the view controller.

