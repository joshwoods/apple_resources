

- Network Extension
-  NEAppPushManager 

Class

# NEAppPushManager

An object that configures a push provider and manages its life cycle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class NEAppPushManager
```

## Mentioned in 

Maintaining a Reliable Network Connection

## Overview

Your app can create as many NEAppPushManager instances as you need. Load your managers from the persistent store and set up their delegates immediately after the app launches, so they’re ready to handle incoming calls.

## Topics

### Matching Wi-Fi networks

var matchSSIDs: [String]

An array of Wi-Fi SSID strings that the system matches for local push activation.

var matchPrivateLTENetworks: [NEPrivateLTENetwork]

An array of private LTE networks that the system matches for local push activation.

class NEPrivateLTENetwork

The parameters of a private LTE network.

### Persisting manager settings

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the manager’s saved configuration from the persistent store.

class func loadAllFromPreferences(completionHandler: ([NEAppPushManager]?, (any Error)?) -> Void)

Loads all saved manager configurations asynchronously.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the manager’s configuration in the persistent store.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the manager’s configuration from the persistent store.

### Working with a delegate

var delegate: (any NEAppPushDelegate)?

A delegate that receives incoming call information from the provider.

protocol NEAppPushDelegate

A protocol that defines how an app push manager instance interacts with the framework.

### Inspecting manager properties

var isActive: Bool

A Boolean value that indicates whether a configuration is in use.

var isEnabled: Bool

A property you use to toggle enabling the configuration.

var localizedDescription: String?

A string that contains the localized description of the app push manager.

### Inspecting provider properties

var providerConfiguration: [String : Any]

A dictionary that contains vendor-specific key-value pairs, that you use to configure a provider.

var providerBundleIdentifier: String?

A string that contains the bundle identifier of the push provider.

### Handling errors

struct NEAppPushManagerError

An error that the push manager encounters.

let NEAppPushErrorDomain: String

The error domain string for local push errors.

enum Code

Error codes that the local push API declares.

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

### Essentials

class NEAppPushProvider

An object that creates and maintains a persistent network connection to a local push server.

Maintaining a Reliable Network Connection

Implement your Local Push Connectivity app to ensure delivery of notifications.

Receiving Voice and Text Communications on a Local Network

Provide voice and text communication on a local network isolated from Apple Push Notification service by adopting Local Push Connectivity.

