

- Network Extension
- NEDNSSettingsManager
-  localizedDescription 

Instance Property

# localizedDescription

A string that contains the display name of the DNS settings configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var localizedDescription: String? { get set }
```

## Discussion

This string is used as the display name of the DNS settings configuration in the system’s settings UI. If this property is set to `nil` at the time that the configuration is created, it is automatically set to the display name of the calling app.

## See Also

### Accessing DNS configuration properties

var isEnabled: Bool

A Boolean you use to query the enabled state of the DNS settings configuration.

var dnsSettings: NEDNSSettings?

An object that contains the configuration settings for a DNS server.

var onDemandRules: [NEOnDemandRule]?

A list of ordered rules that defines the networks on which the DNS settings will apply.

