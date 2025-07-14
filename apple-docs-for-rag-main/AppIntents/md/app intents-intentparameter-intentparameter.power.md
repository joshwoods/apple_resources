

- App Intents
- IntentParameter
-  IntentParameter.Power 

Enumeration

# IntentParameter.Power

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Power
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Power, IntentParameter&lt;Value>.Power) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case femtowatts

case gigawatts

case horsepower

case kilowatts

case megawatts

case microwatts

case milliwatts

case nanowatts

case picowatts

case terawatts

case watts

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

var unit: IntentParameter&lt;Value>.Power?

var defaultUnit: IntentParameter&lt;Value>.Power?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

