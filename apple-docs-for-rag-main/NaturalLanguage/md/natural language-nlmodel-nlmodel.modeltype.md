

- Natural Language
- NLModel
-  NLModel.ModelType 

Enumeration

# NLModel.ModelType

The different types of a natural language model.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum ModelType
```

## Topics

### Model types

case sequence

A sequence model type that tags text at the token level.

case classifier

A classifier model type that tags text at the phrase, sentence, paragraph, or higher level.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the configuration

var language: NLLanguage?

The language the model supports.

var revision: Int

The version of the Natural Language framework that trained the model.

class func supportedRevisions(for: NLModel.ModelType) -> IndexSet

Returns the versions of the Natural Language framework the OS supports.

class func currentRevision(for: NLModel.ModelType) -> Int

Returns the current Natural Language framework version in the OS.

var type: NLModel.ModelType

The natural language model type of the model.

