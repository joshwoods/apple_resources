

- PencilKit
- PKToolPickerCustomItem
- PKToolPickerCustomItem.Configuration
-  toolAttributeControls 

Instance Property

# toolAttributeControls

Defines which attribute controls are available to be presented in UI such as the tool attributes popover, or inline in the picker presented from a pencil squeeze. Controls for properties which the tool item does not support will not be presented. Excluding a control here does not hide all UI for adjusting that value. For example, excluding the opacity control here will not remove it from the color picker, if the color picker is otherwise available. Defaults to all controls.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var toolAttributeControls: PKToolPickerCustomItem.ControlOptions
```

