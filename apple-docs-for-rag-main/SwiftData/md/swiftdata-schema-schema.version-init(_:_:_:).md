

- SwiftData
- Schema
- Schema.Version
-  init(\_:\_:\_:) 

Initializer

# init(\_:\_:\_:)

Initializes a version struct with the provided components of a semantic version.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
init(
    _ major: Int,
    _ minor: Int,
    _ patch: Int
)
```

## Parameters 

`major`  

The major version number.

`minor`  

The minor version number.

`patch`  

The patch version number.

## Discussion

Precondition

`major >= 0 && minor >= 0 && patch >= 0`.

