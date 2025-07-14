

- AppKit
- NSColorPickingDefault
-  minContentSize() 

Instance Method

# minContentSize()

Indicates the receiver’s minimum content size.

macOS 10.5+

``` source
@MainActor
func minContentSize() -> NSSize
```

**Required**

## Discussion

The receiver does not allow a size smaller than `minContentSize`.

## See Also

### Configuring Color Pickers

func setMode(NSColorPanel.Mode)

Specifies the receiver’s mode.

**Required**

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image of a given button cell.

**Required**

func provideNewButtonImage() -> NSImage

Provides the image of the button used to select the receiver in the color panel.

**Required**

func buttonToolTip() -> String

Provides the toolbar button help tag.

**Required**

