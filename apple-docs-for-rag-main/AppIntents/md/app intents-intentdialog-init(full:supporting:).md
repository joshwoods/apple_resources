

- App Intents
- IntentDialog
-  init(full:supporting:) 

Initializer

# init(full:supporting:)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    full: LocalizedStringResource,
    supporting: LocalizedStringResource
)
```

## Discussion

Parameters:

- full: a standalone message that fully describes the output

- supporting: a message that may be used in conjunction with visual output

## See Also

### Creating a dialog

init(LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: String.LocalizationValue.StringInterpolation)

Creates an instance from a string interpolation.

