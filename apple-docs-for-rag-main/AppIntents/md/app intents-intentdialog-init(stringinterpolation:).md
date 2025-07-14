

- App Intents
- IntentDialog
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates an instance from a string interpolation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(stringInterpolation: String.LocalizationValue.StringInterpolation)
```

## Parameters 

`stringInterpolation`  

An instance of `StringInterpolation` which has had each segment of the string literal appended to it.

## Discussion

Most `StringInterpolation` types will store information about the literals and interpolations appended to them in one or more properties. `init(stringInterpolation:)` should use these properties to initialize the instance.

## See Also

### Creating a dialog

init(LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(full: LocalizedStringResource, supporting: LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

