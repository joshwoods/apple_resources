

- Sound Analysis
-  SNClassifierIdentifier 

Structure

# SNClassifierIdentifier

An identifier that represents the versions of the framework’s sound classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SNClassifierIdentifier
```

## Topics

### Selecting a Sound Classifier

static let version1: SNClassifierIdentifier

Version 1 of the sound classifier.

### Creating an Identifier

init(rawValue: String)

Creates an identifier for a sound classifier.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Request

init(mlModel: MLModel) throws

Creates a request that uses a custom sound classification model.

init(classifierIdentifier: SNClassifierIdentifier) throws

Creates a request that uses the framework’s built-in sound classification model.

