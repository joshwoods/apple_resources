

- Network Extension
-  NERelayManager 

Class

# NERelayManager

An object you use to create and manage a network relay configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class NERelayManager
```

## Overview

When your app starts up, access the shared instance of the relay manager, and load existing settings from the preferences using loadFromPreferences(completionHandler:). You can define your relay server configuration, and persist it by calling saveToPreferences(completionHandler:).

## Topics

### Managing relay configurations

class func shared() -> NERelayManager

Access the single instance of a network relay manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your relay configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your relay configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your relay configuration from the system networking preferences.

### Accessing relay configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the relay configuration.

var relays: [NERelay]?

An array of one or two relay server configurations. If multiple relays are configured, application traffic routes through both of them in the order they appear in the array.

var matchDomains: [String]?

A list of domain strings used to determine which connections will use the relay configuration contained in this object.

var excludedDomains: [String]?

A list of domain strings used to determine which connections won’t use the relay configuration contained in this object.

var localizedDescription: String?

A string that contains the display name of the relay configuration.

var onDemandRules: [NEOnDemandRule]?

An array of rules you use to determine which networks the relay uses.

class NEOnDemandRule

A base class shared by all VPN On Demand rules.

### Loading previously-used managers

class func loadAllManagersFromPreferences(completionHandler: ([NERelayManager], (any Error)?) -> Void)

Asynchronously reads all the relay configurations previously created and saved by the calling app.

### Handling errors

let NERelayErrorDomain: String

The domain for errors resulting from calls to the relay manager.

enum NERelayManagerError

Error codes specific to relay managers.

### Instance Properties

var excludedFQDNs: [String]?

var isUIToggleEnabled: Bool

var matchFQDNs: [String]?

### Instance Methods

func getLastClientErrors(TimeInterval, completionHandler: ([any Error]?) -> Void)

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

### Relay configuration

class NERelay

A single relay server configuration that you can chain together with other relays.

