

- Network Extension
-  NEOnDemandRuleIgnore 

Class

# NEOnDemandRuleIgnore

A VPN On Demand rule that doesn’t change the status of the VPN.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEOnDemandRuleIgnore
```

## Overview

When rules of this class match, the VPN connection is not started, and the current status of the VPN connection is left unchanged.

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

class NEOnDemandRuleEvaluateConnection

A VPN On Demand rule that evaluate the app’s connection to determine whether to run its action.

class NEOnDemandRule

A base class shared by all VPN On Demand rules.

