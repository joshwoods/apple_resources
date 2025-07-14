

- Network Extension
-  NEOnDemandRuleDisconnect 

Class

# NEOnDemandRuleDisconnect

A VPN On Demand rule that disconnects the VPN.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEOnDemandRuleDisconnect
```

## Overview

When rules of this class match, the VPN connection is not started, and the VPN connection is disconnected if it is not already disconnected.

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

class NEOnDemandRuleIgnore

A VPN On Demand rule that doesn’t change the status of the VPN.

class NEOnDemandRuleEvaluateConnection

A VPN On Demand rule that evaluate the app’s connection to determine whether to run its action.

class NEOnDemandRule

A base class shared by all VPN On Demand rules.

