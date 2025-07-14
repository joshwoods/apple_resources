

- App Intents
- NegativeAppShortcutPhrase
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates an instance from a string interpolation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(stringInterpolation: NegativeAppShortcutPhrase.StringInterpolation)
```

## Parameters 

`stringInterpolation`  

An instance of `StringInterpolation` which has had each segment of the string literal appended to it.

## Discussion

Most `StringInterpolation` types will store information about the literals and interpolations appended to them in one or more properties. `init(stringInterpolation:)` should use these properties to initialize the instance.

