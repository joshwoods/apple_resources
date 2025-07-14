

- WidgetKit
-  AppIntentControlValueProvider 

Protocol

# AppIntentControlValueProvider

A type that uses a custom intent to provide a value to a control template.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
protocol AppIntentControlValueProvider
```

## Overview

The provider quickly and cheaply prepares a synchronous value to be shown while previewing the control in the add sheet. When the actual control needs to be rendered, the actual, current value will be fetched asynchronously.

The provider prepares these values using an intent containing user-editable parameters.

For instance, a control that opens and closes various doors in a user’s home may show a preview of the door being closed. When the actual control is rendered, the control may fetch the configured door’s status from the cloud:

```
struct DoorValueProvider: AppIntentControlValueProvider {
    func previewValue(configuration: SelectDoorIntent) -> Door {
        Door(id: configuration.doorId, isOpen: false)
    }

    func currentValue(configuration: SelectDoorIntent) async -> Door {
        let isOpen = await DoorManager.shared
            .status(doorId: configuration.doorId)
        return Door(id: configuration.doorId, isOpen: isOpen)
    }
}
```

## Topics

### Associated Types

associatedtype Configuration : ControlConfigurationIntent

The type of intent used to prepare the value.

**Required**

associatedtype Value

The type of value provided to the template.

**Required**

### Instance Methods

func currentValue(configuration: Self.Configuration) async throws -> Self.Value

The current value of the control.

**Required**

func previewValue(configuration: Self.Configuration) -> Self.Value

A value to be shown while previewing the control in the add sheet.

**Required**

## See Also

### Control values and previews

protocol ControlValueProvider

A type that provides a value to a control widget template.

