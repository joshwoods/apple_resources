

- AppKit
- NSImage
-  lockFocus() Deprecated

Instance Method

# lockFocus()

Prepares the image to receive drawing commands.

macOS 10.0–15.4Deprecated

``` source
func lockFocus()
```

Deprecated

Use init(size:flipped:drawingHandler:) instead.

## Discussion

This method sets the current drawing context to the area of the offscreen window used to cache the receiver’s contents. Subsequent drawing commands are composited to this offscreen window. If the offscreen drawing area already has some content, any new drawing commands are composited with that content. This method does not modify the original image data directly.

When locking focus, this method chooses the best image representation object available and locks focus on that object. If the receiver has no image representations, this method creates one with the default depth and locks focus on it. For information on how the “best” representation is chosen, see the Images chapter of Cocoa Drawing Guide.

A successful lockFocus() message must be balanced with a matching unlockFocus() message to the same `NSImage` object. These messages bracket the code that draws the image.

If lockFocus() is unable to focus on the image, it raises an `NSImageCacheException`.

## See Also

### Related Documentation

var isValid: Bool

A Boolean value that indicates whether it is possible to draw an image representation.

var representations: [NSImageRep]

An array containing all of the image object’s image representations.

var prefersColorMatch: Bool

A Boolean value that indicates whether the image prefers to choose image representations using color-matching or resolution-matching.

### Instance Methods

func lockFocusFlipped(Bool)

Prepares the image to receive drawing commands using the specified flipped state.

Deprecated

func unlockFocus()

Removes the focus from the image.

Deprecated

convenience init(iconRef: IconRef)

Initializes the image object with a Carbon-style icon resource.

Deprecated

