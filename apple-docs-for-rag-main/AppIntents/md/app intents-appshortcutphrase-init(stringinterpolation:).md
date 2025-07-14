

- App Intents
- AppShortcutPhrase
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates an instance from a string interpolation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(stringInterpolation: AppShortcutPhrase.StringInterpolation)
```

## Parameters 

`stringInterpolation`  

An instance of `StringInterpolation` which has had each segment of the string literal appended to it.

## Discussion

Most `StringInterpolation` types will store information about the literals and interpolations appended to them in one or more properties. `init(stringInterpolation:)` should use these properties to initialize the instance.

## See Also

### Creating a shortcut phrase

init(String)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

struct StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

enum AppShortcutPhraseToken

Dynamic values you can include in the spoken phrases that run your shortcut.

