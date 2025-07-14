

- Create ML Components
- DatasetError
-  DatasetError.incompatibleDataFormat(\_:debugDescription:) 

Case

# DatasetError.incompatibleDataFormat(\_:debugDescription:)

An error that indicates that a resource doesn’t have the expected data format.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case incompatibleDataFormat(
    URL,
    debugDescription: String
)
```

## See Also

### Analyzing the error

case incorrectName(URL, debugDescription: String)

An error that indicates that a resource has incorrect name format.

case missingResource(URL)

An error that indicates that a resource is missing.

case unreadableResource(URL)

An error that indicates that a resource is unreadable.

var errorDescription: String?

A localized message describing what error occurred.

