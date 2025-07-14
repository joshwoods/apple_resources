

- SwiftUI
- ContentTransition
-  identity 

Type Property

# identity

The identity content transition, which indicates that content changes shouldn’t animate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let identity: ContentTransition
```

## Discussion

You can pass this value to a contentTransition(_:) modifier to selectively disable animations that would otherwise be applied by a withAnimation(_:_:) block.

## See Also

### Getting content transitions

static let interpolate: ContentTransition

A content transition that indicates the views attempt to interpolate their contents during transitions, where appropriate.

static func numericText(countsDown: Bool) -> ContentTransition

Creates a content transition intended to be used with `Text` views displaying numeric text. In certain environments changes to the text will enable a nonstandard transition tailored to numeric characters that count up or down.

static func numericText(value: Double) -> ContentTransition

Creates a content transition intended to be used with `Text` views displaying numbers.

static let opacity: ContentTransition

A content transition that indicates content fades from transparent to opaque on insertion, and from opaque to transparent on removal.

static var symbolEffect: ContentTransition

A content transition that applies the default symbol effect transition to symbol images within the inserted or removed view hierarchy. Other views are unaffected by this transition.

static func symbolEffect&lt;T>(T, options: SymbolEffectOptions) -> ContentTransition

Creates a content transition that applies the symbol Replace animation to symbol images that it is applied to.

