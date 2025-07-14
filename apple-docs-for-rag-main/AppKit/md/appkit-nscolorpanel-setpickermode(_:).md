

- AppKit
- NSColorPanel
-  setPickerMode(\_:) 

Type Method

# setPickerMode(\_:)

Specifies the color panel’s initial picker.

macOS

``` source
@MainActor
class func setPickerMode(_ mode: NSColorPanel.Mode)
```

## Parameters 

`mode`  

A constant specifying which color picker mode is initially visible. This is one of the symbolic constants described in `Color Panel Modes`.

## Discussion

This method may be called at any time, whether or not an application’s `NSColorPanel` has been instantiated.

## See Also

### Setting Color Picker Modes

var mode: NSColorPanel.Mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

enum Mode

A type defined for the `enum` constants specifying color panel modes.

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

struct Options

The color modes that are enabled for a color panel.

