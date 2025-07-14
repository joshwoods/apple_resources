

- Network Extension
-  NEAppPushProvider 

Class

# NEAppPushProvider

An object that creates and maintains a persistent network connection to a local push server.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class NEAppPushProvider
```

## Mentioned in 

Maintaining a Reliable Network Connection

## Overview

Subclass NEAppPushProvider to provide the connection to your local push server. A NEAppPushManager creates instances of your provider class based on the providerBundleIdentifier in the manager’s configuration. The manager then calls methods on your provider to start and stop communication with the server, and periodically check the provider’s status. When your provider receives an incoming call from your server, call the provider’s reportIncomingCall(userInfo:) method to alert the manager’s delegate.

### Creating a Local Push Provider Extension

Local Push Providers run as App Extensions for the `app-push-provider` extension point, which is a possible value the Network Extensions Entitlement.

To create a Local Push Provider extension, first create a new App Extension target in your project.

For an example of an Xcode build target for this app extension, see the Receiving Voice and Text Communications on a Local Network sample code project.

Once you have an extension target, create a subclass of NEAppPushProvider. Then set the `NSExtensionPrincipalClass` key in the extension’s `Info.plist` to the name of your subclass. Set the `NSExtensionPointIdentifier` key in the extension’s `Info.plist` to `com.apple.networkextension.app-push`, if it’s not set already.

Here’s an example of the `NSExtension` dictionary in a Local Push Provider extension’s `Info.plist`:

```
NSExtension

    NSExtensionPointIdentifier
    com.apple.networkextension.app-push
    NSExtensionPrincipalClass
    $(PRODUCT_MODULE_NAME).MyPushProvider

```

Finally, add your Local Push Provider extension target to your app’s Embed App Extensions build phase.

## Topics

### Inspecting provider properties

var providerConfiguration: [String : Any]?

A dictionary that contains current vendor-specific configuration parameters.

### Implementing provider life cycle

func start()

Indicates that the framework has started the provider.

func start(completionHandler: ((any Error)?) -> Void)

Indicates that the framework has started the provider, and provides a completion handler for subclasses to signal their readiness.

func stop(with: NEProviderStopReason, completionHandler: () -> Void)

Indicates that the framework needs to stop the provider.

func handleTimerEvent()

Indicates a periodic status check from the framework to the provider.

### Receiving local events

func reportIncomingCall(userInfo: [AnyHashable : Any])

Informs the manager about an incoming call.

func reportPushToTalkMessage(userInfo: [AnyHashable : Any])

Informs the manager about a push-to-talk message on the connection.

## Relationships

### Inherits From

- NEProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

class NEAppPushManager

An object that configures a push provider and manages its life cycle.

Maintaining a Reliable Network Connection

Implement your Local Push Connectivity app to ensure delivery of notifications.

Receiving Voice and Text Communications on a Local Network

Provide voice and text communication on a local network isolated from Apple Push Notification service by adopting Local Push Connectivity.

