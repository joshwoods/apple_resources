

- Network Extension
- NERelayManager
-  relays 

Instance Property

# relays

An array of one or two relay server configurations. If multiple relays are configured, application traffic routes through both of them in the order they appear in the array.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var relays: [NERelay]? { get set }
```

## See Also

### Accessing relay configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the relay configuration.

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

