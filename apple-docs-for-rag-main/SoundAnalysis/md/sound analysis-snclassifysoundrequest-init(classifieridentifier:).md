

- Sound Analysis
- SNClassifySoundRequest
-  init(classifierIdentifier:) 

Initializer

# init(classifierIdentifier:)

Creates a request that uses the framework’s built-in sound classification model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(classifierIdentifier: SNClassifierIdentifier) throws
```

## Parameters 

`classifierIdentifier`  

A sound classifier version identifier, such as version1.

## Mentioned in 

Classifying Sounds in an Audio File

## See Also

### Creating a Request

init(mlModel: MLModel) throws

Creates a request that uses a custom sound classification model.

struct SNClassifierIdentifier

An identifier that represents the versions of the framework’s sound classifier.

