

- Network Extension
-  NEEvaluateConnectionRuleAction 

Enumeration

# NEEvaluateConnectionRuleAction

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEEvaluateConnectionRuleAction
```

## Topics

### Rule Actions

case connectIfNeeded

Start the VPN if connections to the matching hostname cannot be resolved.

case neverConnect

Do not start the VPN.

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

### Accessing the Rule Action

var action: NEEvaluateConnectionRuleAction

The action to take if the properties of the network connection being established match the rule.

