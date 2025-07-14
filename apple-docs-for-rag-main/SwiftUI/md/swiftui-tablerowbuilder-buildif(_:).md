

- SwiftUI
- TableRowBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Creates a row result for conditional statements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static func buildIf(_ content: C?) -> C? where Value == C.TableRowValue, C : TableRowContent
```

Available when `Value` conforms to `Identifiable`.

## Discussion

This method provides support for “if” statements in multi-statement closures, producing an optional value that is visible only when the condition evaluates to `true`.

## See Also

### Building a row from conditionals

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Creates a row result for the first of two row content alternatives.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Creates a row result for the second of two row content alternatives.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

