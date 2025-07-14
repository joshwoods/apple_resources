

- AppKit
- NSImage
-  init(iconRef:) Deprecated

Initializer

# init(iconRef:)

Initializes the image object with a Carbon-style icon resource.

macOS 10.5–11.0Deprecated

``` source
convenience init(iconRef: IconRef)
```

Deprecated

Use -\[NSWorkspace iconForFile:\], -\[NSWorkspace iconForFiles:\], -\[NSWorkspace iconForFileType:\], or +\[NSImage imageNamed:\] instead.

## Parameters 

`iconRef`  

A reference to a Carbon icon resource.

## Return Value

An initialized `NSImage` object.

## Discussion

Creates one or more bitmap image representations, one for each size icon contained in the `IconRef` data structure. This initialization method automatically retains the data in the `iconRef` parameter and loads the bitmaps from that data file lazily.

## See Also

### Instance Methods

func lockFocus()

Prepares the image to receive drawing commands.

Deprecated

func lockFocusFlipped(Bool)

Prepares the image to receive drawing commands using the specified flipped state.

Deprecated

func unlockFocus()

Removes the focus from the image.

Deprecated

