

- Swift
- ExpressibleByStringInterpolation
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates an instance from a string interpolation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(stringInterpolation: Self.StringInterpolation)
```

**Required** Default implementation provided.

## Parameters 

`stringInterpolation`  

An instance of `StringInterpolation` which has had each segment of the string literal appended to it.

## Discussion

Most `StringInterpolation` types will store information about the literals and interpolations appended to them in one or more properties. `init(stringInterpolation:)` should use these properties to initialize the instance.

## Default Implementations

### ExpressibleByStringInterpolation Implementations

init(stringInterpolation: DefaultStringInterpolation)

Creates a new instance from an interpolated string literal.

