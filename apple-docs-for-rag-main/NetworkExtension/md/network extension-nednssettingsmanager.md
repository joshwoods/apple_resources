

- Network Extension
-  NEDNSSettingsManager 

Class

# NEDNSSettingsManager

An object you use to create and manage a DNS settings configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class NEDNSSettingsManager
```

## Overview

When your app starts up, access the shared instance of the DNS settings manager, and load existing settings from the preferences using loadFromPreferences(completionHandler:). You can define your DNS server configuration, and persist it by calling saveToPreferences(completionHandler:).

In order to use your DNS settings, the user needs to enable it in the Settings app on iOS or in System Preferences on macOS.

## Topics

### Managing DNS configurations

class func shared() -> NEDNSSettingsManager

Access the single instance of a DNS settings manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your DNS settings configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your DNS settings configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your DNS settings configuration from the system networking preferences.

### Accessing DNS configuration properties

var isEnabled: Bool

A Boolean you use to query the enabled state of the DNS settings configuration.

var dnsSettings: NEDNSSettings?

An object that contains the configuration settings for a DNS server.

var localizedDescription: String?

A string that contains the display name of the DNS settings configuration.

var onDemandRules: [NEOnDemandRule]?

A list of ordered rules that defines the networks on which the DNS settings will apply.

### Handling errors

let NEDNSSettingsErrorDomain: String

The domain for errors resulting from calls to the DNS settings manager.

enum NEDNSSettingsManagerError

Error codes specific to DNS managers.

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

### DNS configuration

class NEDNSOverHTTPSSettings

The DNS resolver settings for a DNS-over-HTTPS server.

class NEDNSOverTLSSettings

The DNS resolver settings for a DNS-over-TLS server.

