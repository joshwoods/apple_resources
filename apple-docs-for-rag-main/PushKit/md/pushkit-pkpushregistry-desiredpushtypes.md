

- PushKit
- PKPushRegistry
-  desiredPushTypes 

Instance Property

# desiredPushTypes

Registers the push types for this push registry object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var desiredPushTypes: Set? { get set }
```

## Mentioned in 

Supporting PushKit Notifications in Your App

## Discussion

When you assign a value to this property, the push registry object makes a registration request with the PushKit server. This request is asynchronous, and the success or failure of the request is reported to your registry’s delegate object. For a successful registration, PushKit delivers a push token to the delegate. Use that token to generate push requests from your server.

For a list of push types that you may include in the set, see PKPushType.

## See Also

### Managing the Push Registry

func pushToken(for: PKPushType) -> Data?

Retrieves the locally cached push token for the specified push type.

