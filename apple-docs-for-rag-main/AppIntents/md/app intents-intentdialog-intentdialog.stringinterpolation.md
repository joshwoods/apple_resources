

- App Intents
- IntentDialog
-  IntentDialog.StringInterpolation 

Type Alias

# IntentDialog.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias StringInterpolation = String.LocalizationValue.StringInterpolation
```

## Discussion

The `StringLiteralType` of an interpolation type must match the `StringLiteralType` of the conforming type.

