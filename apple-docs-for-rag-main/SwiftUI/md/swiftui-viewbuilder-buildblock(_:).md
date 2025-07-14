

- SwiftUI
- ViewBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

Passes a single view written as a child view through unmodified.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func buildBlock(_ content: Content) -> Content where Content : View
```

Show all declarations

## Discussion

An example of a single view written as a child view is `{ Text("Hello") }`.

## See Also

### Building content

static func buildBlock() -> EmptyView

Builds an empty view from a block containing no statements.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

