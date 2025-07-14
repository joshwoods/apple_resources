

- App Intents
- IntentParameter
-  IntentParameter.Speed 

Enumeration

# IntentParameter.Speed

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Speed
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Speed, IntentParameter&lt;Value>.Speed) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case kilometersPerHour

case knots

case metersPerSecond

case milesPerHour

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CaseIterable Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable

## See Also

### Accessing unit details

var unit: IntentParameter&lt;Value>.Speed?

var defaultUnit: IntentParameter&lt;Value>.Speed?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

