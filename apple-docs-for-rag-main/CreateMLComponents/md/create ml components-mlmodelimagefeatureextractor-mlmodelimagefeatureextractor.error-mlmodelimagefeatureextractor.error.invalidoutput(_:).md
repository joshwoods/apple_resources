

- Create ML Components
- MLModelImageFeatureExtractor
- MLModelImageFeatureExtractor.Error
-  MLModelImageFeatureExtractor.Error.invalidOutput(\_:) 

Case

# MLModelImageFeatureExtractor.Error.invalidOutput(\_:)

An error indicating that the mlmodel does not produce the required output.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case invalidOutput(String)
```

## See Also

### Analyzing the error

case invalidInput(String)

An error indicating that the mlmodel does not take required input.

var debugDescription: String

A text representation of the error.

