

- Network Extension
- NEOnDemandRule
-  dnsSearchDomainMatch 

Instance Property

# dnsSearchDomainMatch

DNS search domains that identify a network.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var dnsSearchDomainMatch: [String]? { get set }
```

## Discussion

An array of NSString objects. If the current default search domain is equal to one of the strings in this array and all of the other conditions in the rule match, then the rule matches. If this property is nil (the default), then the current default search domain does not factor into the rule match.

## See Also

### Accessing match parameters

var dnsServerAddressMatch: [String]?

DNS server addresses that identify a network.

var interfaceTypeMatch: NEOnDemandRuleInterfaceType

An interface type to identify a network.

enum NEOnDemandRuleInterfaceType

var ssidMatch: [String]?

SSIDs that identify a network.

var probeURL: URL?

A URL to probe when all other network identifiers match to validate that an expected resource is available.

