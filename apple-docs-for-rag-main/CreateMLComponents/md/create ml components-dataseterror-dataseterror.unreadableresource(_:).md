

- Create ML Components
- DatasetError
-  DatasetError.unreadableResource(\_:) 

Case

# DatasetError.unreadableResource(\_:)

An error that indicates that a resource is unreadable.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case unreadableResource(URL)
```

## See Also

### Analyzing the error

case incompatibleDataFormat(URL, debugDescription: String)

An error that indicates that a resource doesn’t have the expected data format.

case incorrectName(URL, debugDescription: String)

An error that indicates that a resource has incorrect name format.

case missingResource(URL)

An error that indicates that a resource is missing.

var errorDescription: String?

A localized message describing what error occurred.

