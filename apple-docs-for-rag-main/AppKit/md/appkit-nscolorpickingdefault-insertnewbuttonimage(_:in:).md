

- AppKit
- NSColorPickingDefault
-  insertNewButtonImage(\_:in:) 

Instance Method

# insertNewButtonImage(\_:in:)

Sets the image of a given button cell.

macOS

``` source
@MainActor
func insertNewButtonImage(
    _ newButtonImage: NSImage,
    in buttonCell: NSButtonCell
)
```

**Required**

## Parameters 

`newButtonImage`  

The image to set for the button cell.

`buttonCell`  

The `NSButtonCell` object that lets the user choose the picker from the color panel—the color picker’s representation in the `NSMatrix` of the `NSColorPanel`.

## Discussion

This method should perform application-specific manipulation of the image before it’s inserted and displayed by the button cell.

## See Also

### Configuring Color Pickers

func setMode(NSColorPanel.Mode)

Specifies the receiver’s mode.

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

