

- Speech
-  SFCustomLanguageModelData 

Class

# SFCustomLanguageModelData

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+

``` source
class SFCustomLanguageModelData
```

## Topics

### Initializers

init(locale: Locale, identifier: String, version: String)

convenience init(locale: Locale, identifier: String, version: String, builder: () -> any DataInsertable)

### Instance Properties

let identifier: String

let locale: Locale

let version: String

### Instance Methods

func export(to: URL) async throws

func insert(phraseCount: SFCustomLanguageModelData.PhraseCount)

func insert(phraseCountGenerator: SFCustomLanguageModelData.PhraseCountGenerator)

func insert(term: SFCustomLanguageModelData.CustomPronunciation)

### Type Methods

static func supportedPhonemes(locale: Locale) -> [String]

### Classes

class PhraseCountGenerator

class TemplatePhraseCountGenerator

### Structures

struct CompoundTemplate

struct CustomPronunciation

struct DataInsertableBuilder

struct PhraseCount

struct PhraseCountsFromTemplates

struct TemplateInsertableBuilder

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Classes

class SFSpeechLanguageModel

class Configuration

