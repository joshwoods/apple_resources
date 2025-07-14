

- PushKit
-  PKPushRegistry 

Class

# PKPushRegistry

An object that requests the delivery and handles the receipt of PushKit notifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class PKPushRegistry
```

## Mentioned in 

Supporting PushKit Notifications in Your App

Responding to VoIP Notifications from PushKit

## Overview

A `PKPushRegistry` object manages only certain types of notifications, such as high-priority notifications needed by a VoIP app. PushKit wakes up your app as needed to deliver incoming notifications and delivers the notifications directly to the push registry object that requested them.

Every time your app launches, whether in the foreground or in the background, create a push registry object and configure it. Typically, you keep the push registry object running for the duration of your app. Each push registry object delivers incoming notifications to its delegate object, which also handles the responses for registration requests. Listing 1 shows how to create a push registry object and request VoIP notifications. Always assign an appropriate delegate object before modifying the desiredPushTypes property.

Listing 1. Creating and configuring a push registry object

- Swift
- Objective-C

```
```

```
```

Assigning a new value to the desiredPushTypes property registers the push registry object with the PushKit servers. The server reports the success or failure of your registration attempts asynchronously to the push registry, which then reports those results to its delegate object. The push registry also delivers all received notifications to the delegate object. For more information about the delegate methods, see PKPushRegistryDelegate.

## Topics

### Initializing a Push Registry

init(queue: dispatch_queue_t?)

Creates a push registry with the specified dispatch queue.

### Receiving the Notification Data

var delegate: (any PKPushRegistryDelegate)?

The delegate object that receives notifications coming from the push registry object.

protocol PKPushRegistryDelegate

The methods that you use to handle incoming PushKit notifications and registration events.

### Managing the Push Registry

var desiredPushTypes: Set&lt;PKPushType>?

Registers the push types for this push registry object.

func pushToken(for: PKPushType) -> Data?

Retrieves the locally cached push token for the specified push type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Registration

Supporting PushKit Notifications in Your App

Declare the types of PushKit notifications your app supports and configure objects to respond to them.

protocol PKPushRegistryDelegate

The methods that you use to handle incoming PushKit notifications and registration events.

class PKPushCredentials

An object that encapsulates the device token you use to deliver push notifications to your app.

