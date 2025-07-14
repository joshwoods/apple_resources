

- SwiftUI
-  ControlWidgetConfigurationBuilder 

Structure

# ControlWidgetConfigurationBuilder

A custom attribute that constructs a control widget’s body.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@resultBuilder
struct ControlWidgetConfigurationBuilder
```

## Overview

The `@ControlWidgetConfigurationBuilder` attribute allows your control widget’s body closure to produce a control widget configuration after zero or more other statements:

```
struct GarageDoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        let kind = "com.yourcompany.GarageDoorOpener"

        StaticControlConfiguration(
            kind: kind
        ) {
            ...
        }
    }
}
```

## Topics

### Type Methods

static func buildBlock&lt;Content>(Content) -> some ControlWidgetConfiguration

Passes a single control widget configuration written as a child control through unmodified.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

## See Also

### Composing control widgets

protocol ControlWidget

The configuration and content of a control widget to display in system spaces such as Control Center, the Lock Screen, and the Action Button.

protocol ControlWidgetConfiguration

A type that describes a control widget’s content.

struct EmptyControlWidgetConfiguration

An empty control widget configuration.

protocol ControlWidgetTemplate

A type that describes a control widget’s content.

struct EmptyControlWidgetTemplate

An empty control widget template.

struct ControlWidgetTemplateBuilder

A custom attribute that constructs a control widget template’s body.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

func controlWidgetStatus(_:)

The status of the control described by the modified label.

