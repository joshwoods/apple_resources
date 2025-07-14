

- SwiftUI
- TableRowBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds an expression within the builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
static func buildExpression(_ content: Content) -> Content where Value == Content.TableRowValue, Content : TableRowContent
```

## See Also

### Building a row from conditionals

static func buildIf&lt;C>(C?) -> C?

Creates a row result for conditional statements.

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Creates a row result for the first of two row content alternatives.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Creates a row result for the second of two row content alternatives.

