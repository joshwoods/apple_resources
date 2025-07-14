

- App Intents
- IntentParameter
-  IntentParameter.Pressure 

Enumeration

# IntentParameter.Pressure

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Pressure
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Pressure, IntentParameter&lt;Value>.Pressure) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case bars

case gigapascals

case hectopascals

case inchesOfMercury

case kilopascals

case megapascals

case millibars

case millimetersOfMercury

case newtonsPerMetersSquared

case poundsForcePerSquareInch

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

var unit: IntentParameter&lt;Value>.Pressure?

var defaultUnit: IntentParameter&lt;Value>.Pressure?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

