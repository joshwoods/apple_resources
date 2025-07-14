

- App Intents
- IntentParameter
-  IntentParameter.ElectricCurrent 

Enumeration

# IntentParameter.ElectricCurrent

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum ElectricCurrent
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.ElectricCurrent, IntentParameter&lt;Value>.ElectricCurrent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case amperes

case kiloamperes

case megaamperes

case microamperes

case milliamperes

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

var unit: IntentParameter&lt;Value>.ElectricCurrent?

var defaultUnit: IntentParameter&lt;Value>.ElectricCurrent?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

