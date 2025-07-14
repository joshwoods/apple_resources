

- HomeKit
- HMActionSet
-  actionSetType 

Instance Property

# actionSetType

The type of the action set, such as built-in or user-defined.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var actionSetType: String { get }
```

## Discussion

An action set type can be user-defined, trigger-owned, or one of the built-in types. Note that built-in action sets cannot be removed from the home, and trigger-owned action sets cannot be executed, renamed, or associated with another trigger.

## See Also

### Specifying a type

Action Set Types

The types of action sets that you can define.

