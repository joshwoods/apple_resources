

- StoreKit
- SKCloudServiceController
-  requestUserToken(forDeveloperToken:completionHandler:) Deprecated

Instance Method

# requestUserToken(forDeveloperToken:completionHandler:)

Returns a user token that you use to access personalized Apple Music content.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func requestUserToken(
    forDeveloperToken developerToken: String,
    completionHandler: @escaping (String?, (any Error)?) -> Void
)
```

``` source
func requestUserToken(forDeveloperToken developerToken: String) async throws -> String
```

Deprecated

Use MusicKit

## Parameters 

`developerToken`  

A signed and encrypted JWT token used to authenticate the developer in Apple Music API requests.

`completionHandler`  

A completion block that includes the following parameters:

userToken  
A token that identifies the user.

error  
The error that occurred, if any.

## Discussion

Use this method with your developer token to get a token that authenticates the user in personalized Apple Music API requests. Note that personalized requests return user-specific data. Errors 401 and 403 only occur when requesting a music user token. They do not occur for any of the other Apple Music API requests.

## See Also

### Determining capabilities

Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

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

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

