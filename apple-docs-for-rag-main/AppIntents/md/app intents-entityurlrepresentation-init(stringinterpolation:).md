

- App Intents
- EntityURLRepresentation
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates an instance from a string interpolation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(stringInterpolation: EntityURLRepresentation.StringInterpolation)
```

## Parameters 

`stringInterpolation`  

An instance of `StringInterpolation` which has had each segment of the string literal appended to it.

## Discussion

Most `StringInterpolation` types will store information about the literals and interpolations appended to them in one or more properties. `init(stringInterpolation:)` should use these properties to initialize the instance.

