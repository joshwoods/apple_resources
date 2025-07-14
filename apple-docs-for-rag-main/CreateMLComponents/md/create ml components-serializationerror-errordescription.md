

- Create ML Components
- SerializationError
-  errorDescription 

Instance Property

# errorDescription

A localized message describing what error occurred.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var errorDescription: String? { get }
```

## See Also

### Analyzing the error

case notRepresentableAsCoreML(debugDescription: String)

An error that indicates that the transformer cannot be represented as a CoreML model.

case packageAlreadyExists(URL)

An error that indicates that the package already exists at the URL.

case packageNotFound(URL)

An error that indicates that the package at specified URL was not found.

