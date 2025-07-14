

- SwiftUI
- WidgetBundleBuilder
-  buildLimitedAvailability(\_:) 

Type Method

# buildLimitedAvailability(\_:)

Builds an availability check within the builder

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
static func buildLimitedAvailability(_ widget: some ControlWidget) -> any Widget & _LimitedAvailabilityWidgetMarker
```

Show all declarations

## See Also

### Bundling widgets

static func buildBlock() -> some Widget

Builds an empty Widget from a block containing no statements, `{ }`.

static buildBlock(_:)

Builds a single Widget written as a child view (e..g, `{ MyWidget() }`) through unmodified.

static buildExpression(_:)

Builds an expression within the builder.

static func buildOptional((any Widget &amp; _LimitedAvailabilityWidgetMarker)?) -> some Widget

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

