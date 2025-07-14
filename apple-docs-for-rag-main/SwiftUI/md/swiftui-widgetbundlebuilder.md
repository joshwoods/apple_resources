

- SwiftUI
-  WidgetBundleBuilder 

Structure

# WidgetBundleBuilder

A custom attribute that constructs a widget bundle’s body.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
struct WidgetBundleBuilder
```

## Overview

Use the `@WidgetBundleBuilder` attribute to group multiple widgets listed in the body property of a widget bundle. For example, the following code defines a widget bundle that consists of two widgets.

```
@main
struct GameWidgets: WidgetBundle {
   @WidgetBundleBuilder
   var body: some Widget {
       GameStatusWidget()
       CharacterDetailWidget()
   }
}
```

## Topics

### Bundling widgets

static func buildBlock() -> some Widget

Builds an empty Widget from a block containing no statements, `{ }`.

static buildBlock(_:)

Builds a single Widget written as a child view (e..g, `{ MyWidget() }`) through unmodified.

static buildExpression(_:)

Builds an expression within the builder.

static buildLimitedAvailability(_:)

Builds an availability check within the builder

static func buildOptional((any Widget &amp; _LimitedAvailabilityWidgetMarker)?) -> some Widget

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

## See Also

### Implementing a widget bundle

var body: Self.Body

Declares the group of widgets that an app supports.

**Required**

associatedtype Body : Widget

The type of widget that represents the content of the bundle.

**Required**

