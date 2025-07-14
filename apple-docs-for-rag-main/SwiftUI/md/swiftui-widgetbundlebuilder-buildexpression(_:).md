

- SwiftUI
- WidgetBundleBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds an expression within the builder.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildExpression(_ content: Content) -> Content where Content : Widget
```

Show all declarations

## See Also

### Bundling widgets

static func buildBlock() -> some Widget

Builds an empty Widget from a block containing no statements, `{ }`.

static buildBlock(_:)

Builds a single Widget written as a child view (e..g, `{ MyWidget() }`) through unmodified.

static buildLimitedAvailability(_:)

Builds an availability check within the builder

static func buildOptional((any Widget &amp; _LimitedAvailabilityWidgetMarker)?) -> some Widget

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

