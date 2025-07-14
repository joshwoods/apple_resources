

- Network Extension
- NEOnDemandRule
-  dnsServerAddressMatch 

Instance Property

# dnsServerAddressMatch

DNS server addresses that identify a network.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var dnsServerAddressMatch: [String]? { get set }
```

## Discussion

An array of DNS server IP addresses represented as `NSString` objects. If each of the current default DNS servers is equal to one of the strings in this array and all of the other conditions in the rule match, then the rule matches. If this property is nil (the default), then the default DNS servers do not factor into the rule match.

## See Also

### Accessing match parameters

var dnsSearchDomainMatch: [String]?

DNS search domains that identify a network.

var interfaceTypeMatch: NEOnDemandRuleInterfaceType

An interface type to identify a network.

enum NEOnDemandRuleInterfaceType

var ssidMatch: [String]?

SSIDs that identify a network.

var probeURL: URL?

A URL to probe when all other network identifiers match to validate that an expected resource is available.

