

- AppKit
- NSColorPickingDefault
-  init(pickerMask:colorPanel:) 

Initializer

# init(pickerMask:colorPanel:)

Initializes the receiver with a given color panel and its mode.

macOS

``` source
@MainActor
init?(
    pickerMask mask: Int,
    colorPanel owningColorPanel: NSColorPanel
)
```

**Required**

## Parameters 

`mask`  

A mask indicating the various color picker modes supported by the color panel. This is determined by the argument to the `NSColorPanel` method setPickerMask(_:). If it has not been set, `panelModes` is `NSColorPanelAllModesMask`. If your color picker supports any additional modes, you should invoke the setPickerMask(_:) method when your application initializes to notify the `NSColorPanel` class. The standard mode constants are defined in Choosing the Color Pickers in a Color Panel.

`owningColorPanel`  

The color panel than owns the receiver.

## Return Value

If your color picker responds to any of the modes represented in `panelModes`, it should perform its initialization and return an initialized color picker. Color pickers that do so have their buttons inserted in the color panel and continue to receive messages from the panel as the user manipulates it. If the color picker doesn’t respond to any of the modes represented in `panelModes`, it should do nothing and return `nil`.

## Discussion

This method is sent by the `NSColorPanel` to all implementors of the color-picking protocols when the application’s color panel is first initialized. In order for your color picker to receive this message, it must have a bundle in your application’s “ColorPickers” directory (described in Adding Custom Color Pickers to a Color Panel).

This method should examine the mask and determine whether it supports any of the modes included there. You may also check the value in `mask` to enable or disable any subpickers or optional controls implemented by your color picker. Your color picker may also retain `owningColorPanel` in an instance variable for future communication with the color panel.

This method is provided to initialize your color picker; however, much of a color picker’s initialization may be done lazily through the `NSColorPickingCustom` protocol’s provideNewView(_:) method.

## See Also

### Related Documentation

Color Programming Topics

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

