

- App Intents
- AppShortcutParameterPresentationSummaryString
- AppShortcutParameterPresentationSummaryString.StringInterpolation
-  appendLiteral(\_:) 

Instance Method

# appendLiteral(\_:)

Appends a literal segment to the interpolation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func appendLiteral(_ literal: String)
```

## Parameters 

`literal`  

A string literal containing the characters that appear next in the string literal.

## Discussion

Don’t call this method directly. Instead, initialize a variable or constant using a string literal with interpolated expressions.

Interpolated expressions don’t pass through this method; instead, Swift selects an overload of `appendInterpolation`. For more information, see the top-level `StringInterpolationProtocol` documentation.

