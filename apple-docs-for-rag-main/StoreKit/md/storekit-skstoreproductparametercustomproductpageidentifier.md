

- StoreKit
-  SKStoreProductParameterCustomProductPageIdentifier 

Global Variable

# SKStoreProductParameterCustomProductPageIdentifier

The key that represents the custom product page identifier you want the store to display when you present the view controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+

``` source
let SKStoreProductParameterCustomProductPageIdentifier: String
```

## Discussion

The value for this key is a UUID that represents a custom product page. Get this value from the `ppid` parameter of your custom product page’s URL. For example, in the following sample custom product page URL:

`https://apps.apple.com/us/app/example-appname/id1234567890?ppid=eb2b3606-2fef-4aab-a54e-b2e5547c9bc3`

- the custom product page identifier is the string that follows `ppid=`, which is `eb2b3606-2fef-4aab-a54e-b2e5547c9bc3`.

App Store Connect creates the URL when you configure your custom product page. For more information, see Create custom product pages.

For more information about custom product pages, see Custom product pages on the App Store.

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

let SKStoreProductParameterProviderToken: String

The key representing the provider token for the developer that created the app specified by the SKStoreProductParameterITunesItemIdentifier key.

