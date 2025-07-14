

- AppKit
- NSColorPanel
-  setPickerMask(\_:) 

Type Method

# setPickerMask(\_:)

Determines which color selection modes are available in an application’s `NSColorPanel`.

macOS

``` source
@MainActor
class func setPickerMask(_ mask: NSColorPanel.Options)
```

## Parameters 

`mask`  

One or more logically ORed color mode masks described in `Color Picker Mode Masks`.

## Discussion

This method has an effect only before an `NSColorPanel` object is instantiated.

If you create a class that implements the color-picking protocols (`NSColorPickingDefault` and `NSColorPickingCustom`), you may want to give it a unique mask—one different from those defined for the standard color pickers. To display your color picker, your application will need to logically OR that unique mask with the standard color mask constants when invoking this method.

## See Also

### Setting Color Picker Modes

class func setPickerMode(NSColorPanel.Mode)

Specifies the color panel’s initial picker.

var mode: NSColorPanel.Mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

enum Mode

A type defined for the `enum` constants specifying color panel modes.

struct Options

The color modes that are enabled for a color panel.

