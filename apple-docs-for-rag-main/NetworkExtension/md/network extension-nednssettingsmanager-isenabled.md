

- Network Extension
- NEDNSSettingsManager
-  isEnabled 

Instance Property

# isEnabled

A Boolean you use to query the enabled state of the DNS settings configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var isEnabled: Bool { get }
```

## Discussion

A user must enable your DNS settings configuration in order to apply it to the system. By default, configurations are disabled until the user enables the configuration in the Settings app on iOS or in System Preferences on macOS.

## See Also

### Accessing DNS configuration properties

var dnsSettings: NEDNSSettings?

An object that contains the configuration settings for a DNS server.

var localizedDescription: String?

A string that contains the display name of the DNS settings configuration.

var onDemandRules: [NEOnDemandRule]?

A list of ordered rules that defines the networks on which the DNS settings will apply.

