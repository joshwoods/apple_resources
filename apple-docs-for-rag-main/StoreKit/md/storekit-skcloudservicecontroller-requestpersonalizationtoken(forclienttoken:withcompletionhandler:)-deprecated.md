

- StoreKit
- SKCloudServiceController
-  requestPersonalizationToken(forClientToken:withCompletionHandler:) Deprecated

Instance Method

# requestPersonalizationToken(forClientToken:withCompletionHandler:)

iOS 10.3–11.0DeprecatediPadOS 10.3–11.0DeprecatedtvOS 10.3–11.0Deprecated

``` source
func requestPersonalizationToken(
    forClientToken clientToken: String,
    withCompletionHandler completionHandler: @escaping (String?, (any Error)?) -> Void
)
```

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

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

Deprecated

