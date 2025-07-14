

- App Intents
- IntentParameter
-  IntentParameter.Area 

Enumeration

# IntentParameter.Area

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Area
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Area, IntentParameter&lt;Value>.Area) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case acres

case ares

case hectares

case squareCentimeters

case squareFeet

case squareInches

case squareKilometers

case squareMegameters

case squareMeters

case squareMicrometers

case squareMiles

case squareMillimeters

case squareNanometers

case squareYards

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

var unit: IntentParameter&lt;Value>.Area?

var defaultUnit: IntentParameter&lt;Value>.Area?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

