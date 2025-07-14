

- PushKit
-  PKPushCredentials 

Class

# PKPushCredentials

An object that encapsulates the device token you use to deliver push notifications to your app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class PKPushCredentials
```

## Mentioned in 

Supporting PushKit Notifications in Your App

## Overview

When registering your app’s push types, PushKit creates a `PKPushCredentials` object for each type your app supports and delivers it to your delegate’s pushRegistry(_:didUpdate:for:) method. Don’t create `PKPushCredentials` objects yourself.

## Topics

### Getting the Token

var token: Data

A unique device token to use when sending push notifications to the current device.

var type: PKPushType

The push type constant associated with the token.

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

class PKPushRegistry

An object that requests the delivery and handles the receipt of PushKit notifications.

protocol PKPushRegistryDelegate

The methods that you use to handle incoming PushKit notifications and registration events.

