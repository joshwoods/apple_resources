

- WidgetKit
-  ControlValueProvider 

Protocol

# ControlValueProvider

A type that provides a value to a control widget template.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
protocol ControlValueProvider
```

## Overview

The provider quickly and cheaply prepares a synchronous value to be shown while previewing the control in the add sheet. When the actual control needs to be rendered, the actual, current value will be fetched asynchronously.

For instance, a control that opens and closes a garage door may show a preview of the door being closed. When the actual control is rendered, the control may fetch the door’s status from the cloud:

```
struct GarageDoorValueProvider: ControlValueProvider {
    var previewValue: Bool { false }

    func currentValue() async -> Bool {
        await GarageDoorManager.shared.doorStatus()
    }
}
```

## Topics

### Associated Types

associatedtype Value

The type of value provided to the template.

**Required**

### Instance Properties

var previewValue: Self.Value

A value to be shown while previewing the control in the add sheet.

**Required**

### Instance Methods

func currentValue() async throws -> Self.Value

The current value of the control.

**Required**

## See Also

### Control values and previews

protocol AppIntentControlValueProvider

A type that uses a custom intent to provide a value to a control template.

