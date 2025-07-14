

- AppKit
- NSImage
-  lockFocusFlipped(\_:) Deprecated

Instance Method

# lockFocusFlipped(\_:)

Prepares the image to receive drawing commands using the specified flipped state.

macOS 10.6–15.4Deprecated

``` source
func lockFocusFlipped(_ flipped: Bool)
```

Deprecated

Use init(size:flipped:drawingHandler:) instead.

## Parameters 

`flipped`  

true if the drawing context should be flipped, otherwise false.

## See Also

### Instance Methods

func lockFocus()

Prepares the image to receive drawing commands.

Deprecated

func unlockFocus()

Removes the focus from the image.

Deprecated

convenience init(iconRef: IconRef)

Initializes the image object with a Carbon-style icon resource.

Deprecated

