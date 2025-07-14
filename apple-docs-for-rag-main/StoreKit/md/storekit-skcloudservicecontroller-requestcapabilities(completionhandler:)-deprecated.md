

- StoreKit
- SKCloudServiceController
-  requestCapabilities(completionHandler:) Deprecated

Instance Method

# requestCapabilities(completionHandler:)

Gets the current capabilities associated with the Music library on the device.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func requestCapabilities(completionHandler: @escaping (SKCloudServiceCapability, (any Error)?) -> Void)
```

``` source
func requestCapabilities() async throws -> SKCloudServiceCapability
```

Deprecated

Use MusicSubscription.current from MusicKit

## Parameters 

`completionHandler`  

A block that is called when the device’s current capabilities are determined. The block takes the following parameters:

capabilities  
Flags that indicate the device’s capabilities. For possible values, see SKCloudServiceCapability.

error  
An error value that indicates the reason for failure. Possible values are SKError.Code.unknown, SKError.Code.cloudServicePermissionDenied, and SKError.Code.cloudServiceNetworkConnectionFailed.

## Mentioned in 

Offering Apple Music Subscription in Your App

Determining a person’s Apple Music capabilities

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestCapabilities() async throws -> SKCloudServiceCapability
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

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

struct SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

Deprecated

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

Deprecated

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

