

- StoreKit
- SKCloudServiceController
-  requestStorefrontIdentifier(completionHandler:) Deprecated

Instance Method

# requestStorefrontIdentifier(completionHandler:)

Gets the device’s storefront identifier.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func requestStorefrontIdentifier(completionHandler: @escaping (String?, (any Error)?) -> Void)
```

``` source
func requestStorefrontIdentifier() async throws -> String
```

Deprecated

Use Storefront.current.id

## Parameters 

`completionHandler`  

A block that is called when the storefront ID is returned. The block takes the following parameters:

storefrontIdentifier  
The identifier of a specific storefront.

error  
An error value that indicates the reason for failure. Possible values are SKError.Code.unknown, SKError.Code.cloudServicePermissionDenied, and SKError.Code.cloudServiceNetworkConnectionFailed.

## Discussion

You need to get the appropriate storefront before you specify a product, because product identifiers are meaningful within the context of a store.

## See Also

### Determining capabilities

Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

func requestUserToken(forDeveloperToken: String, completionHandler: (String?, (any Error)?) -> Void)

Returns a user token that you use to access personalized Apple Music content.

Deprecated

func requestStorefrontCountryCode(completionHandler: (String?, (any Error)?) -> Void)

Gets the country code for the storefront associated with a customer’s iTunes account.

Deprecated

func requestCapabilities(completionHandler: (SKCloudServiceCapability, (any Error)?) -> Void)

Gets the current capabilities associated with the Music library on the device.

Deprecated

struct SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

Deprecated

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

