

- SwiftUI
- ContentTransition
-  numericText(value:) 

Type Method

# numericText(value:)

Creates a content transition intended to be used with `Text` views displaying numbers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func numericText(value: Double) -> ContentTransition
```

## Parameters 

`value`  

The value represented by the `Text` view being animated. The difference between the old and new values when the text changes will be used to determine the animation direction.

## Return Value

A new content transition.

## Discussion

The example below creates a text view displaying a particular value, assigning the same value to the associated transition:

```
Text("\(value)")
    .contentTransition(.numericText(value: value))
```

## See Also

### Getting content transitions

static let identity: ContentTransition

The identity content transition, which indicates that content changes shouldn’t animate.

static let interpolate: ContentTransition

A content transition that indicates the views attempt to interpolate their contents during transitions, where appropriate.

static func numericText(countsDown: Bool) -> ContentTransition

Creates a content transition intended to be used with `Text` views displaying numeric text. In certain environments changes to the text will enable a nonstandard transition tailored to numeric characters that count up or down.

static let opacity: ContentTransition

A content transition that indicates content fades from transparent to opaque on insertion, and from opaque to transparent on removal.

static var symbolEffect: ContentTransition

A content transition that applies the default symbol effect transition to symbol images within the inserted or removed view hierarchy. Other views are unaffected by this transition.

static func symbolEffect&lt;T>(T, options: SymbolEffectOptions) -> ContentTransition

Creates a content transition that applies the symbol Replace animation to symbol images that it is applied to.

