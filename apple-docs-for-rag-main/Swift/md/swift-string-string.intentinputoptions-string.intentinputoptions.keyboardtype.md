

- Swift
- String
- String.IntentInputOptions
-  String.IntentInputOptions.KeyboardType 

Enumeration

# String.IntentInputOptions.KeyboardType

Describes the types of keyboard to use for text entry.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum KeyboardType
```

## Topics

### Operators

static func == (String.IntentInputOptions.KeyboardType, String.IntentInputOptions.KeyboardType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case URL

A keyboard that provides URL entry.

case asciiCapable

A keyboard that displays standard ASCII characters.

case `default`

case numberPad

A numeric keypad.

case numbersAndPunctuation

A keyboard that displays numbers and punctuation.

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

