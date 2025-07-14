

- Network Extension
- NEDNSSettingsManager
-  onDemandRules 

Instance Property

# onDemandRules

A list of ordered rules that defines the networks on which the DNS settings will apply.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var onDemandRules: [NEOnDemandRule]? { get set }
```

## Discussion

An On Demand rule with the action NEOnDemandRuleAction.connect defines a network on which the DNS settings apply. An On Demand rule with the action NEOnDemandRuleAction.disconnect causes DNS settings to not apply. An On Demand rule with the action of NEOnDemandRuleAction.evaluateConnection can be used to enable the DNS settings on a network with excluded domains, as specified using a NEEvaluateConnectionRuleAction.neverConnect rule.

## See Also

### Accessing DNS configuration properties

var isEnabled: Bool

A Boolean you use to query the enabled state of the DNS settings configuration.

var dnsSettings: NEDNSSettings?

An object that contains the configuration settings for a DNS server.

var localizedDescription: String?

A string that contains the display name of the DNS settings configuration.

