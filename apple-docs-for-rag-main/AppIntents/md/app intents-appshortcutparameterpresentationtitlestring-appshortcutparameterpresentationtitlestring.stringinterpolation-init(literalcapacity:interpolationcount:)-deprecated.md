

- App Intents
- AppShortcutParameterPresentationTitleString
- AppShortcutParameterPresentationTitleString.StringInterpolation
-  init(literalCapacity:interpolationCount:) Deprecated

Initializer

# init(literalCapacity:interpolationCount:)

Creates an empty instance ready to be filled with string literal content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+visionOS 1.0+

``` source
init(
    literalCapacity: Int,
    interpolationCount: Int
)
```

Deprecated

Please use init(for:summary:optionsCollections:)

## Parameters 

`literalCapacity`  

The approximate size of all literal segments combined. This is meant to be passed to `String.reserveCapacity(_:)`; it may be slightly larger or smaller than the sum of the counts of each literal segment.

`interpolationCount`  

The number of interpolations which will be appended. Use this value to estimate how much additional capacity will be needed for the interpolated segments.

## Discussion

Don’t call this initializer directly. Instead, initialize a variable or constant using a string literal with interpolated expressions.

Swift passes this initializer a pair of arguments specifying the size of the literal segments and the number of interpolated segments. Use this information to estimate the amount of storage you will need.

