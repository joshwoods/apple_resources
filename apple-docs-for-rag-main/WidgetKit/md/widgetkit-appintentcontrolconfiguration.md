

- WidgetKit
-  AppIntentControlConfiguration 

Structure

# AppIntentControlConfiguration

The description of a control widget that uses a custom intent to provide user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
struct AppIntentControlConfiguration where Configuration : ControlConfigurationIntent, Content : ControlWidgetTemplate
```

## Overview

The following example shows the configuration for a door opener control able to open a door specified by the user.

```
struct DoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        AppIntentControlConfiguration(
            kind: "com.yourcompany.GarageDoorOpener",
            provider: DoorValueProvider()
        ) { door in
            ControlWidgetToggle(
                door.name,
                isOn: door.isOpen,
                action: ToggleDoor(door)
            ) {
                Label(
                    $0 ? "Open" : "Closed",
                    systemImage: $0 ? "door.open" : "door.closed"
                )
            }
        }
    }
}
```

Every control has a unique `kind`, a string that you choose. You use this string to identify your control when reloading its template with ControlCenter.

The value provider is an object that determines a value to use to render your template. This provider receives an intent containing user-editable parameters.

The content closure defines the template that WidgetKit needs to render the control. If you create the configuration using a value provider, when WidgetKit invokes the content closure, it passes a value created by the provider’s `AppIntentControlValueProvider/previewValue` property or `AppIntentControlValueProvider/currentValue()` function.

## Topics

### Initializers

init(kind: String, intent: Configuration.Type, content: (Configuration) -> Content)

Creates a configuration for a control widget by using a custom intent to provide user-configurable options.

init&lt;Provider>(kind: String, provider: Provider, content: (Provider.Value) -> Content)

Creates a configuration for a control widget by using a custom intent to provide user-configurable options.

## Relationships

### Conforms To

- ControlWidgetConfiguration
- Sendable

## See Also

### Control configuration

struct StaticControlConfiguration

The description of a control widget that has no user-configurable options.

struct ControlInfo

A structure that contains information about user-configured controls.

