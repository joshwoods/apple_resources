

- SwiftUI
- ControlWidgetConfiguration
-  pushHandler(\_:) 

Instance Method

# pushHandler(\_:)

Register a type that can handle push tokens changing for controls of this type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func pushHandler(_ pushHandlerType: any ControlPushHandler.Type) -> some ControlWidgetConfiguration
```

## Discussion

Use this to opt your control into using push notifications.

If you have multiple control types, you can choose to use the same push handler type for those control types.

When the push configuration of your controls changes, each handler type will be instantiated and `PushHandler/pushTokensDidChange(controls:)` will be called.

