

- App Intents
- IntentParameter
-  IntentParameter.Length 

Enumeration

# IntentParameter.Length

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Length
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.Length, IntentParameter&lt;Value>.Length) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case astronomicalUnits

case centimeters

case decameters

case decimeters

case fathoms

case feet

case furlongs

case hectometers

case inches

case kilometers

case lightyears

case megameters

case meters

case micrometers

case miles

case millimeters

case nanometers

case nauticalMiles

case parsecs

case picometers

case scandinavianMiles

case yards

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

var unit: IntentParameter&lt;Value>.Length?

var defaultUnit: IntentParameter&lt;Value>.Length?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

