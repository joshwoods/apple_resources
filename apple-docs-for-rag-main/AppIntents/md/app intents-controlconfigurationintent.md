

- App Intents
-  ControlConfigurationIntent 

Protocol

# ControlConfigurationIntent

An interface for configuring a Control Center module.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
protocol ControlConfigurationIntent : AppIntent
```

## Overview

The parameters of your intent define all of the configuration options for your control.

```
struct SelectFocusIntent: ControlConfigurationIntent {
    static let title: LocalizedStringResource = "Select Focus"
    static let description: IntentDescription = "Turn Focus on to silence notifications and filter out distractions."

    struct FocusOptionsProvider: DynamicOptionsProvider {
        func results() async throws -> [Focus] {
            FocusManager.shared.allFocuses
        }
    }

    @Parameter(title: "Focus", default: .doNotDisturb, optionsProvider: FocusOptionsProvider())
    var focus: Focus
}
```

When using this protocol, you don’t need to provide an implementation for perform(). You can, however, still implement `perform()` to use the same implementation for both control configuration and as an actionable intent.

The example above provides a default value for the `focus` intent parameter. By providing a default value, you can use a non-optional value for the intent parameter. If you don’t provide a default value for the intent parameter, the parameter’s value must be optional, to allow the system to preview the control before someone configures it.

## Topics

### Associated Types

associatedtype NeverResult

**Required**

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

## See Also

### Controls, widgets, and Live Activities

protocol LiveActivityStartingIntent

An intent that starts, pauses, or otherwise modifies a Live Activity.

Deprecated

protocol LiveActivityIntent

An intent that starts, pauses, or otherwise modifies a Live Activity when it runs.

protocol WidgetConfigurationIntent

An interface for configuring a WidgetKit widget.

