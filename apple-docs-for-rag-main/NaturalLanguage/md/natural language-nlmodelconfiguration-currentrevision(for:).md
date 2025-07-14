

- Natural Language
- NLModelConfiguration
-  currentRevision(for:) 

Type Method

# currentRevision(for:)

Returns the current Natural Language framework version in the OS.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class func currentRevision(for type: NLModel.ModelType) -> Int
```

## Return Value

A version number.

## See Also

### Accessing the configuration

var language: NLLanguage?

The language the model supports.

var revision: Int

The version of the Natural Language framework that trained the model.

class func supportedRevisions(for: NLModel.ModelType) -> IndexSet

Returns the versions of the Natural Language framework the OS supports.

var type: NLModel.ModelType

The natural language model type of the model.

enum ModelType

The different types of a natural language model.

