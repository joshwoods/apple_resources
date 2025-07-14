

- WidgetKit
-  StaticControlConfiguration 

Structure

# StaticControlConfiguration

The description of a control widget that has no user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
struct StaticControlConfiguration where Content : ControlWidgetTemplate
```

## Overview

The following example shows the configuration for a garage door opener control.

```
struct GarageDoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        StaticControlConfiguration(
            kind: "com.yourcompany.GarageDoorOpener",
            provider: GarageDoorValueProvider()
        ) { isOpen in
            ControlWidgetToggle(
                "Garage Door",
                isOn: isOpen,
                action: ToggleGarageDoor()
            ) {
                Label(
                    $0 ? "Open" : "Closed",
                    systemImage: $0 ? "door.garage.open" : "door.garage.closed"
                )
            }
        }
    }
}
```

Every control has a unique `kind`, a string that you choose to uniquely identify the type of control. You use this string to identify your control when reloading its template with ControlCenter.

The value provider is an object that determines a value to use to render your template.

The content closure defines the template that WidgetKit needs to render the control. If you create the configuration using a value provider, when WidgetKit invokes the content closure, it passes a value created by the provider’s previewValue property or currentValue() function.

## Topics

### Initializers

init(kind: String, content: () -> Content)

Creates a configuration for a control, with no user-configurable options.

init&lt;Provider>(kind: String, provider: Provider, content: (Provider.Value) -> Content)

Creates a configuration for a control, with no user-configurable options.

## Relationships

### Conforms To

- ControlWidgetConfiguration
- Sendable

## See Also

### Control configuration

struct AppIntentControlConfiguration

The description of a control widget that uses a custom intent to provide user-configurable options.

struct ControlInfo

A structure that contains information about user-configured controls.

