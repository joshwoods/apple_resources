

- Swift
- EncodingError
- EncodingError.Context
-  init(codingPath:debugDescription:underlyingError:) 

Initializer

# init(codingPath:debugDescription:underlyingError:)

Creates a new context with the given path of coding keys and a description of what went wrong.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    codingPath: [any CodingKey],
    debugDescription: String,
    underlyingError: (any Error)? = nil
)
```

## Parameters 

`codingPath`  

The path of coding keys taken to get to the point of the failing encode call.

`debugDescription`  

A description of what went wrong, for debugging purposes.

`underlyingError`  

The underlying error which caused this error, if any.

