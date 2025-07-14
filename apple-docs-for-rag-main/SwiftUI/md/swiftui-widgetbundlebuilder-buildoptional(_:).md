

- SwiftUI
- WidgetBundleBuilder
-  buildOptional(\_:) 

Type Method

# buildOptional(\_:)

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildOptional(_ widget: (any Widget & _LimitedAvailabilityWidgetMarker)?) -> some Widget
```

## Discussion

Conditional statements in a WidgetBundleBuilder can contain an `if` statement but not an `else` statement, and the condition can only perform a compiler check for availability, like in the following code:

```
var body: some Widget {
    if #available(iOS 16, *) {
        WindowGroup {
            ContentView()
        }
    }
}
```

## See Also

### Bundling widgets

static func buildBlock() -> some Widget

Builds an empty Widget from a block containing no statements, `{ }`.

static buildBlock(_:)

Builds a single Widget written as a child view (e..g, `{ MyWidget() }`) through unmodified.

static buildExpression(_:)

Builds an expression within the builder.

static buildLimitedAvailability(_:)

Builds an availability check within the builder

