

- App Intents
- IntentDialog
-  init(\_:) 

Initializer

# init(\_:)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ string: LocalizedStringResource)
```

## Discussion

Parameters:

- string: a standalone message that fully describes the output

## See Also

### Creating a dialog

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: String.LocalizationValue.StringInterpolation)

Creates an instance from a string interpolation.

init(full: LocalizedStringResource, supporting: LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

