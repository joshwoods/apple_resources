

- Network Extension
-  NEOnDemandRuleInterfaceType 

Enumeration

# NEOnDemandRuleInterfaceType

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEOnDemandRuleInterfaceType
```

## Topics

### Interface Types

case any

Match any interface type

case ethernet

Match wired ethernet interfaces

case wiFi

Match Wi-Fi interfaces

case cellular

Match cellular data interfaces

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing match parameters

var dnsSearchDomainMatch: [String]?

DNS search domains that identify a network.

var dnsServerAddressMatch: [String]?

DNS server addresses that identify a network.

var interfaceTypeMatch: NEOnDemandRuleInterfaceType

An interface type to identify a network.

var ssidMatch: [String]?

SSIDs that identify a network.

var probeURL: URL?

A URL to probe when all other network identifiers match to validate that an expected resource is available.

