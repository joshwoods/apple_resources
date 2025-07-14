

- Swift
- String
- String.IntentInputOptions
-  String.IntentInputOptions.CapitalizationType 

Enumeration

# String.IntentInputOptions.CapitalizationType

Describes the capitalization modes to apply to text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum CapitalizationType
```

## Topics

### Operators

static func == (String.IntentInputOptions.CapitalizationType, String.IntentInputOptions.CapitalizationType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case allCharacters

A mode that capitalizes all characters.

case none

A mode that applies no automatic capitalization.

case sentences

A mode that capitalizes the first letter of each sentence.

case words

A mode that capitalizes the first letter of each word.

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

