

- Network Extension
-  NEFilterRule 

Class

# NEFilterRule

A rule for filters that combines a rule to match network traffic and an action to take when the rule matches.

macOS 10.15+

``` source
class NEFilterRule
```

## Topics

### Creating a Filter Rule

init(networkRule: NENetworkRule, action: NEFilterAction)

Creates a new filter rule from a network rule and an action to take when network traffic matches.

### Inspecting Filter Rule Properties

var networkRule: NENetworkRule

The network rule that defines the network traffic characteristics that this filter rule matches.

var action: NEFilterAction

The action to take when this rule matches network traffic.

## Relationships

### Inherits From

- NSObject

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

### Creating Filter Settings

init(rules: [NEFilterRule], defaultAction: NEFilterAction)

Creates a new settings instance from an array of rules and a default action.

