

- App Intents
- IntentParameter
-  IntentParameter.Volume 

Enumeration

# IntentParameter.Volume

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Volume
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Volume, IntentParameter&lt;Value>.Volume) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case acreFeet

case bushels

case centiliters

case cubicCentimeters

case cubicDecimeters

case cubicFeet

case cubicInches

case cubicKilometers

case cubicMeters

case cubicMiles

case cubicMillimeters

case cubicYards

case cups

case deciliters

case fluidOunces

case gallons

case imperialFluidOunces

case imperialGallons

case imperialPints

case imperialQuarts

case imperialTablespoons

case imperialTeaspoons

case kiloliters

case liters

case megaliters

case metricCups

case milliliters

case pints

case quarts

case tablespoons

case teaspoons

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

var unit: IntentParameter&lt;Value>.Volume?

var defaultUnit: IntentParameter&lt;Value>.Volume?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

