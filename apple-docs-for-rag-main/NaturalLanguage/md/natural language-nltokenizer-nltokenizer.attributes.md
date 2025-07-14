

- Natural Language
- NLTokenizer
-  NLTokenizer.Attributes 

Structure

# NLTokenizer.Attributes

Hints about the contents of the string for the tokenizer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct Attributes
```

## Topics

### Contents

static var emoji: NLTokenizer.Attributes

The string contains emoji.

static var numeric: NLTokenizer.Attributes

The string contains numbers.

static var symbolic: NLTokenizer.Attributes

The string contains symbols.

### Initializers

init(rawValue: UInt)

Creates an attribute with given value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring a tokenizer

var string: String?

The text to be tokenized.

func setLanguage(NLLanguage)

Sets the language of the text to be tokenized.

var unit: NLTokenUnit

The linguistic unit that this tokenizer uses.

