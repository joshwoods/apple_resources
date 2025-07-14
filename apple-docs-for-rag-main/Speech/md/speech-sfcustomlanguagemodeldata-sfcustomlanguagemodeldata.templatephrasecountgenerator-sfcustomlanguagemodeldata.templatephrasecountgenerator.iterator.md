

- Speech
- SFCustomLanguageModelData
- SFCustomLanguageModelData.TemplatePhraseCountGenerator
-  SFCustomLanguageModelData.TemplatePhraseCountGenerator.Iterator 

Class

# SFCustomLanguageModelData.TemplatePhraseCountGenerator.Iterator

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+

``` source
class Iterator
```

## Topics

### Type Aliases

typealias Element

### Initializers

init(templates: [SFCustomLanguageModelData.TemplatePhraseCountGenerator.Template], templateClasses: [String : [String]])

### Instance Methods

func next() async throws -> SFCustomLanguageModelData.PhraseCount?

## Relationships

### Inherits From

- SFCustomLanguageModelData.PhraseCountGenerator.Iterator

### Conforms To

- AsyncIteratorProtocol

