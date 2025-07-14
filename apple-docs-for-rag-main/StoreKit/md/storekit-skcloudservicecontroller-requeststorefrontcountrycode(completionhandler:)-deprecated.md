

- StoreKit
- SKCloudServiceController
-  requestStorefrontCountryCode(completionHandler:) Deprecated

Instance Method

# requestStorefrontCountryCode(completionHandler:)

Gets the country code for the storefront associated with a customer’s iTunes account.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func requestStorefrontCountryCode(completionHandler: @escaping (String?, (any Error)?) -> Void)
```

``` source
func requestStorefrontCountryCode() async throws -> String
```

Deprecated

Use MusicDataRequest.currentCountryCode from MusicKit

## Parameters 

`completionHandler`  

A block that is called when the storefront country code is returned. The block takes the following parameters:

storefrontCountryCode  
The country code of a specific storefront.

error  
An error value that indicates the reason for failure. See SKError.Code for possible error values.

## Discussion

You need to get the appropriate storefront country code before you specify a product as each country or region contains different products.

## See Also

### Determining capabilities

Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

func requestUserToken(forDeveloperToken: String, completionHandler: (String?, (any Error)?) -> Void)

Returns a user token that you use to access personalized Apple Music content.

Deprecated

func requestCapabilities(completionHandler: (SKCloudServiceCapability, (any Error)?) -> Void)

Gets the current capabilities associated with the Music library on the device.

Deprecated

struct SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

Deprecated

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

Deprecated

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

