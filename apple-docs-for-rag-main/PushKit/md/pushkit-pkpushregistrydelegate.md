

- PushKit
-  PKPushRegistryDelegate 

Protocol

# PKPushRegistryDelegate

The methods that you use to handle incoming PushKit notifications and registration events.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
protocol PKPushRegistryDelegate : NSObjectProtocol
```

## Overview

Implement the methods of this protocol in an object of your app and assign that object to the delegate property of your `PKPushRegistry` object. Use the methods of this protocol to process incoming notifications and to react to token registration and invalidation.

## Topics

### Responding to Registration Events

func pushRegistry(PKPushRegistry, didUpdate: PKPushCredentials, for: PKPushType)

Tells the delegate that the system updated the credentials for the specified type of push notification.

**Required**

func pushRegistry(PKPushRegistry, didInvalidatePushTokenFor: PKPushType)

Tells the delegate that the system invalidated the push token for the specified type.

### Handling an Incoming Notification

func pushRegistry(PKPushRegistry, didReceiveIncomingPushWith: PKPushPayload, for: PKPushType, completion: () -> Void)

Tells the delegate that a remote push notification arrived.

### Deprecated Methods

func pushRegistry(PKPushRegistry, didReceiveIncomingPushWith: PKPushPayload, for: PKPushType)

Notifies the delegate that a remote push has been received.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Registration

Supporting PushKit Notifications in Your App

Declare the types of PushKit notifications your app supports and configure objects to respond to them.

class PKPushRegistry

An object that requests the delivery and handles the receipt of PushKit notifications.

class PKPushCredentials

An object that encapsulates the device token you use to deliver push notifications to your app.

