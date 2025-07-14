

- Natural Language
- NLModelConfiguration
-  type 

Instance Property

# type

The natural language model type of the model.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var type: NLModel.ModelType { get }
```

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

enum ModelType

The different types of a natural language model.

