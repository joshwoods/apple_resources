

- AppKit
- NSImage
-  unlockFocus() Deprecated

Instance Method

# unlockFocus()

Removes the focus from the image.

macOS 10.0–15.4Deprecated

``` source
func unlockFocus()
```

Deprecated

Use init(size:flipped:drawingHandler:) instead.

## Discussion

This message must be sent after a successful lockFocus() or lockFocusOnRepresentation: message and the completion of any intermediate drawing commands. This method restores the focus to the previous owner, if any.

Do not send this message if the preceding call to lock focus raised an `NSImageCacheException`.

## See Also

### Instance Methods

func lockFocus()

Prepares the image to receive drawing commands.

Deprecated

func lockFocusFlipped(Bool)

Prepares the image to receive drawing commands using the specified flipped state.

Deprecated

convenience init(iconRef: IconRef)

Initializes the image object with a Carbon-style icon resource.

Deprecated

