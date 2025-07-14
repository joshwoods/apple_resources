

- App Intents
- IntentParameter
-  IntentParameter.DateKind 

Enumeration

# IntentParameter.DateKind

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum DateKind
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.DateKind, IntentParameter&lt;Value>.DateKind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case date

case dateTime

case time

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

### Accessing the date kind

var dateKind: IntentParameter&lt;Value>.DateKind?

