

- App Intents
- IntentParameter
-  IntentParameter.ConcentrationMass 

Enumeration

# IntentParameter.ConcentrationMass

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum ConcentrationMass
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.ConcentrationMass, IntentParameter&lt;Value>.ConcentrationMass) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case gramsPerLiter

case milligramsPerDeciliter

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

var unit: IntentParameter&lt;Value>.ConcentrationMass?

var defaultUnit: IntentParameter&lt;Value>.ConcentrationMass?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

