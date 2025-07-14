

- Network Extension
-  NEOnDemandRuleEvaluateConnection 

Class

# NEOnDemandRuleEvaluateConnection

A VPN On Demand rule that evaluate the app’s connection to determine whether to run its action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEOnDemandRuleEvaluateConnection
```

## Overview

When rules of this class match, the properties of the network connection being established are matched against a set of connection rules. The action of the matched rule (if any) is used to determine whether or not the VPN will be started.

## Topics

### Accessing connection rules

var connectionRules: [NEEvaluateConnectionRule]?

An array of NEEvaluateConnectionRule objects

class NEEvaluateConnectionRule

`NEEvaluateConnectionRule` associates properties of network connections with an action.

## Relationships

### Inherits From

- NEOnDemandRule

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

class NEOnDemandRule

A base class shared by all VPN On Demand rules.

