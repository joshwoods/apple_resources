

- AppKit
- NSColorPickingDefault
-  buttonToolTip() 

Instance Method

# buttonToolTip()

Provides the toolbar button help tag.

macOS 10.5+

``` source
@MainActor
func buttonToolTip() -> String
```

**Required**

## Return Value

Help tag text.

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

func minContentSize() -> NSSize

Indicates the receiver’s minimum content size.

**Required**

