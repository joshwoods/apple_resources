

- StoreKit
- SKCloudServiceSetupViewController
-  load(options:completionHandler:) Deprecated

Instance Method

# load(options:completionHandler:)

Loads the cloud service setup view with the specified options.

iOS 10.1–18.0DeprecatediPadOS 10.1–18.0DeprecatedMac Catalyst 13.1–18.0Deprecated

``` source
@MainActor
func load(
    options: [SKCloudServiceSetupOptionsKey : Any] = [:],
    completionHandler: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func load(options: [SKCloudServiceSetupOptionsKey : Any] = [:]) async throws -> Bool
```

Deprecated

Use the musicSubscriptionOffer(isPresented:options:onLoadCompletion:) SwiftUI View Modifier from MusicKit

## Parameters 

`options`  

A key that identifies the type of setup the user needs to do. See SKCloudServiceSetupOptionsKey for possible values.

`completionHandler`  

A block that is called when the setup view has loaded. The block takes the following parameters:

`result`

A Boolean value that indicates whether the view controller has loaded the view and can be presented.

`error`

An error value that indicates the reason for failure. Possible values are SKError.Code.unknown, SKError.Code.cloudServicePermissionDenied, and SKError.Code.cloudServiceNetworkConnectionFailed.

## Mentioned in 

Offering Apple Music Subscription in Your App

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func load(options: [SKCloudServiceSetupOptionsKey : Any] = [:]) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading the setup view

Offering Apple Music Subscription in Your App

Allow eligible customers to subscribe to Apple Music.

struct SKCloudServiceSetupOptionsKey

Keys to specify the types of setup options for a cloud service.

class SKArcadeService

