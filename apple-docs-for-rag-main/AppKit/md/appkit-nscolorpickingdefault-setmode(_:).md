

- AppKit
- NSColorPickingDefault
-  setMode(\_:) 

Instance Method

# setMode(\_:)

Specifies the receiver’s mode.

macOS

``` source
@MainActor
func setMode(_ mode: NSColorPanel.Mode)
```

**Required**

## Parameters 

`mode`  

The color picker mode. The available modes are described in Choosing the Color Pickers in a Color Panel.

## Discussion

This method is invoked by the `NSColorPanel` method mode method to ensure the color picker reflects the current mode. For example, invoke this method during color picker initialization to ensure that all color pickers are restored to the mode the user left them in the last time an `NSColorPanel` was used.

Most color pickers have only one mode and thus don’t need to do any work in this method. An example of a color picker that uses this method is the slider picker, which can choose from one of several submodes depending on the value of `mode`.

## See Also

### Configuring Color Pickers

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image of a given button cell.

**Required**

func provideNewButtonImage() -> NSImage

Provides the image of the button used to select the receiver in the color panel.

**Required**

func minContentSize() -> NSSize

Indicates the receiver’s minimum content size.

**Required**

func buttonToolTip() -> String

Provides the toolbar button help tag.

**Required**

