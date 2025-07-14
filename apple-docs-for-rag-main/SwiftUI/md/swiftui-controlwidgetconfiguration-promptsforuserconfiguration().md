

- SwiftUI
- ControlWidgetConfiguration
-  promptsForUserConfiguration() 

Instance Method

# promptsForUserConfiguration()

Specifies that a control’s configuration UI should be automatically presented after the widget is added.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func promptsForUserConfiguration() -> some ControlWidgetConfiguration
```

## Return Value

A control configuration that knows whether the presentation of a configuration UI is preferred.

