

- Speech
- SFCustomLanguageModelData
-  SFCustomLanguageModelData.TemplatePhraseCountGenerator 

Class

# SFCustomLanguageModelData.TemplatePhraseCountGenerator

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+

``` source
class TemplatePhraseCountGenerator
```

## Topics

### Initializers

init()

init(from: any Decoder) throws

### Instance Methods

func define(className: String, values: [String])

func hash(into: inout Hasher)

func insert(template: String, count: Int)

func makeAsyncIterator() -> SFCustomLanguageModelData.PhraseCountGenerator.Iterator

### Operator Functions

static func == (SFCustomLanguageModelData.TemplatePhraseCountGenerator, SFCustomLanguageModelData.TemplatePhraseCountGenerator) -> Bool

### Classes

class Iterator

### Structures

struct Template

## Relationships

### Inherits From

- SFCustomLanguageModelData.PhraseCountGenerator

### Conforms To

- AsyncSequence
- DataInsertable
- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Classes

class PhraseCountGenerator

