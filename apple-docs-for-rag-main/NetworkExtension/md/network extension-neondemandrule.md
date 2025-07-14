

- Network Extension
-  NEOnDemandRule 

Class

# NEOnDemandRule

A base class shared by all VPN On Demand rules.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEOnDemandRule
```

## Overview

Each rule is defined by a single action and a set of optional matching conditions. The action defines how the system should trigger the VPN when the conditions are met, such as connecting automatically for all connections, connecting conditionally, or disconnecting. The optional conditions describe parameters of a network. Some common rules include disconnecting the VPN on a trusted, internal network, and triggering on all other networks. When rules are defined in an array, they are evaluated in order and the action of the first rule to match all conditions is chosen.

Instances of the `NEOnDemandRule` class should be created through one of its subclasses: NEOnDemandRuleConnect, NEOnDemandRuleDisconnect, NEOnDemandRuleEvaluateConnection, or NEOnDemandRuleIgnore.

## Topics

### Accessing match parameters

var dnsSearchDomainMatch: [String]?

DNS search domains that identify a network.

var dnsServerAddressMatch: [String]?

DNS server addresses that identify a network.

var interfaceTypeMatch: NEOnDemandRuleInterfaceType

An interface type to identify a network.

enum NEOnDemandRuleInterfaceType

var ssidMatch: [String]?

SSIDs that identify a network.

var probeURL: URL?

A URL to probe when all other network identifiers match to validate that an expected resource is available.

### Accessing the rule action

var action: NEOnDemandRuleAction

The action of the On Demand Rule.

enum NEOnDemandRuleAction

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEOnDemandRuleConnect
- NEOnDemandRuleDisconnect
- NEOnDemandRuleEvaluateConnection
- NEOnDemandRuleIgnore

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Settings

class NEOnDemandRuleConnect

A VPN On Demand rule that connects the VPN.

class NEOnDemandRuleDisconnect

A VPN On Demand rule that disconnects the VPN.

class NEOnDemandRuleIgnore

A VPN On Demand rule that doesn’t change the status of the VPN.

class NEOnDemandRuleEvaluateConnection

A VPN On Demand rule that evaluate the app’s connection to determine whether to run its action.

