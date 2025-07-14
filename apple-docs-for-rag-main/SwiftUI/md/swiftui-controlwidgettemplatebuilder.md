

- SwiftUI
-  ControlWidgetTemplateBuilder 

Structure

# ControlWidgetTemplateBuilder

A custom attribute that constructs a control widget template’s body.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@resultBuilder
struct ControlWidgetTemplateBuilder
```

## Overview

The `@ControlWidgetTemplateBuilder` attribute allows your control template’s body closure to produce a control template after zero or more other statements:

```
struct GarageDoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        let kind = "com.yourcompany.GarageDoorOpener"

        StaticControlConfiguration(
            kind: kind
        ) {
            let isOpen = ...

            ControlWidgetToggle(
                "Garage Door",
                isOn: isOpen,
                action: ToggleGarageDoor()
            ) {
                Label(
                    $0 ? "Open" : "Closed",
                    systemImage: $0 ?
                        "door.garage.open" : "door.garage.closed"
                )
            }
        }
    }
}
```

## Topics

### Type Methods

static func buildBlock&lt;Content>(Content) -> some ControlWidgetTemplate

Passes a single control widget template written as a child view through unmodified.

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

struct ControlWidgetConfigurationBuilder

A custom attribute that constructs a control widget’s body.

protocol ControlWidgetTemplate

A type that describes a control widget’s content.

struct EmptyControlWidgetTemplate

An empty control widget template.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

func controlWidgetStatus(_:)

The status of the control described by the modified label.

