

- Network Extension
- NEOnDemandRule
-  interfaceTypeMatch 

Instance Property

# interfaceTypeMatch

An interface type to identify a network.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var interfaceTypeMatch: NEOnDemandRuleInterfaceType { get set }
```

## Discussion

The type of interface that this rule matches. If the current primary network interface is of this type and all of the other conditions in the rule match, then the rule matches. If this property is `NEOnDemandRuleInterfaceTypeAny` (the default), then the current primary interface type does not factor into the rule match.

## See Also

### Accessing match parameters

var dnsSearchDomainMatch: [String]?

DNS search domains that identify a network.

var dnsServerAddressMatch: [String]?

DNS server addresses that identify a network.

enum NEOnDemandRuleInterfaceType

var ssidMatch: [String]?

SSIDs that identify a network.

var probeURL: URL?

A URL to probe when all other network identifiers match to validate that an expected resource is available.

