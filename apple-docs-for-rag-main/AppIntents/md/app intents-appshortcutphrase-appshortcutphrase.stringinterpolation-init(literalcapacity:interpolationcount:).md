

- App Intents
- AppShortcutPhrase
- AppShortcutPhrase.StringInterpolation
-  init(literalCapacity:interpolationCount:) 

Initializer

# init(literalCapacity:interpolationCount:)

Creates an empty instance ready to be filled with string literal content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    literalCapacity: Int,
    interpolationCount: Int
)
```

## Parameters 

`literalCapacity`  

The approximate size of all literal segments combined. This is meant to be passed to `String.reserveCapacity(_:)`; it may be slightly larger or smaller than the sum of the counts of each literal segment.

`interpolationCount`  

The number of interpolations which will be appended. Use this value to estimate how much additional capacity will be needed for the interpolated segments.

## Discussion

Don’t call this initializer directly. Instead, initialize a variable or constant using a string literal with interpolated expressions.

Swift passes this initializer a pair of arguments specifying the size of the literal segments and the number of interpolated segments. Use this information to estimate the amount of storage you will need.

