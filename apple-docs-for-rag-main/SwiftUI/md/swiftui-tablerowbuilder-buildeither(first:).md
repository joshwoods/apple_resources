

- SwiftUI
- TableRowBuilder
-  buildEither(first:) 

Type Method

# buildEither(first:)

Creates a row result for the first of two row content alternatives.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static func buildEither(first: T) -> _ConditionalContent where Value == T.TableRowValue, T : TableRowContent, F : TableRowContent, T.TableRowValue == F.TableRowValue
```

Available when `Value` conforms to `Identifiable`.

## Discussion

This method provides support for “if” statements in multi-statement closures, producing conditional content for the “then” branch.

## See Also

### Building a row from conditionals

static func buildIf&lt;C>(C?) -> C?

Creates a row result for conditional statements.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Creates a row result for the second of two row content alternatives.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

