

- AppKit
- NSColorPickingDefault
-  provideNewButtonImage() 

Instance Method

# provideNewButtonImage()

Provides the image of the button used to select the receiver in the color panel.

macOS

``` source
@MainActor
func provideNewButtonImage() -> NSImage
```

**Required**

## Return Value

The image for the mode button the user uses to select this picker in the color panel; that is, the color picker’s representation in the `NSMatrix` of the `NSColorPanel`.

## Discussion

This image is the same one the color panel uses as an argument when sending the insertNewButtonImage(_:in:) message.

## See Also

### Configuring Color Pickers

func setMode(NSColorPanel.Mode)

Specifies the receiver’s mode.

**Required**

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image of a given button cell.

**Required**

func minContentSize() -> NSSize

Indicates the receiver’s minimum content size.

**Required**

func buttonToolTip() -> String

Provides the toolbar button help tag.

**Required**

