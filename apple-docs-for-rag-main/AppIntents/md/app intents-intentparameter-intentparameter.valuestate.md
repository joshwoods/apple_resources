

- App Intents
- IntentParameter
-  IntentParameter.ValueState 

Enumeration

# IntentParameter.ValueState

Indicates whether an IntentParameter was provided an initial value or if it was unset

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
enum ValueState
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Topics

### Enumeration Cases

case set(Value)

The parameter was provided an initial value.

case unset

The parameter was never provided a value

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable

