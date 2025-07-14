

- App Intents
- IntentParameter
-  IntentParameter.IntControlStyle 

Enumeration

# IntentParameter.IntControlStyle

An enum that describes the control style of an Integer parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum IntControlStyle
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.IntControlStyle, IntentParameter&lt;Value>.IntControlStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case field

case stepper

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Accessing the control style

var controlStyle: IntentParameter&lt;Value>.IntControlStyle?

