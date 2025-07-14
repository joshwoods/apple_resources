

- DockKit
- DockAccessory
- DockAccessory.AccessoryEvent
-  DockAccessory.AccessoryEvent.button(id:pressed:) 

Case

# DockAccessory.AccessoryEvent.button(id:pressed:)

A button press event on the dock accessory.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
case button(
    id: Int,
    pressed: Bool
)
```

## Parameters 

`id`  

A unique, vendor-specific identifier for the given button.

`pressed`  

`true` on button press down, `false` on button release up.

