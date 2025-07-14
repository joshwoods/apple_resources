

- Network Extension
- NEDNSSettingsManager
-  dnsSettings 

Instance Property

# dnsSettings

An object that contains the configuration settings for a DNS server.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var dnsSettings: NEDNSSettings? { get set }
```

## Discussion

This property can be set to either an NEDNSOverHTTPSSettings object or an NEDNSOverTLSSettings object.

## See Also

### Accessing DNS configuration properties

var isEnabled: Bool

A Boolean you use to query the enabled state of the DNS settings configuration.

var localizedDescription: String?

A string that contains the display name of the DNS settings configuration.

var onDemandRules: [NEOnDemandRule]?

A list of ordered rules that defines the networks on which the DNS settings will apply.

