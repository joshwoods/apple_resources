

- Natural Language
- NLModelConfiguration
-  supportedRevisions(for:) 

Type Method

# supportedRevisions(for:)

Returns the versions of the Natural Language framework the OS supports.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class func supportedRevisions(for type: NLModel.ModelType) -> IndexSet
```

## Return Value

An index set of version numbers.

## See Also

### Accessing the configuration

var language: NLLanguage?

The language the model supports.

var revision: Int

The version of the Natural Language framework that trained the model.

class func currentRevision(for: NLModel.ModelType) -> Int

Returns the current Natural Language framework version in the OS.

var type: NLModel.ModelType

The natural language model type of the model.

enum ModelType

The different types of a natural language model.

