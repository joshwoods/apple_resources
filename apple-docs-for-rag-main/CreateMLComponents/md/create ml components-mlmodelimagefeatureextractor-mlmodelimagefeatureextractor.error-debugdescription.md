

- Create ML Components
- MLModelImageFeatureExtractor
- MLModelImageFeatureExtractor.Error
-  debugDescription 

Instance Property

# debugDescription

A text representation of the error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var debugDescription: String { get }
```

## See Also

### Analyzing the error

case invalidInput(String)

An error indicating that the mlmodel does not take required input.

case invalidOutput(String)

An error indicating that the mlmodel does not produce the required output.

