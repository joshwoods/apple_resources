

- System
- FilePath
- FilePath.Component
-  init(stringLiteral:) 

Initializer

# init(stringLiteral:)

Create a file path component from a string literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(stringLiteral: String)
```

## Discussion

Precondition: `stringLiteral` is non-empty, is not a root, and has only one component in it.

