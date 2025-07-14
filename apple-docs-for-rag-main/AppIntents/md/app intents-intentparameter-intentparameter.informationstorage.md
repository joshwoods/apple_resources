

- App Intents
- IntentParameter
-  IntentParameter.InformationStorage 

Enumeration

# IntentParameter.InformationStorage

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum InformationStorage
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Topics

### Operators

static func == (IntentParameter&lt;Value>.InformationStorage, IntentParameter&lt;Value>.InformationStorage) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case bits

case bytes

case exabits

case exabytes

case exbibits

case exbibytes

case gibibits

case gibibytes

case gigabits

case gigabytes

case kibibits

case kibibytes

case kilobits

case kilobytes

case mebibits

case mebibytes

case megabits

case megabytes

case nibbles

case pebibits

case pebibytes

case petabits

case petabytes

case tebibits

case tebibytes

case terabits

case terabytes

case yobibits

case yobibytes

case yottabits

case yottabytes

case zebibits

case zebibytes

case zettabits

case zettabytes

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

var unit: IntentParameter&lt;Value>.InformationStorage?

var defaultUnit: IntentParameter&lt;Value>.InformationStorage?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

