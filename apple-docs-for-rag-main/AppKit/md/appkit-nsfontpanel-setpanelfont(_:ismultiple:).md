

- AppKit
- NSFontPanel
-  setPanelFont(\_:isMultiple:) 

Instance Method

# setPanelFont(\_:isMultiple:)

Sets the selected font in the receiver to the specified font.

macOS

``` source
@MainActor
func setPanelFont(
    _ fontObj: NSFont,
    isMultiple flag: Bool
)
```

## Parameters 

`fontObj`  

The font to be selected.

`flag`  

If false, selects the specified font; otherwise selects no font and displays a message in the preview area indicating that multiple fonts are selected.

## Discussion

You normally don’t use this method directly; instead, you send setSelectedFont(_:isMultiple:) to the shared `NSFontManager`, which in turn invokes this method.

