

- WatchKit
- WKImageAnimatable
-  startAnimating() 

Instance Method

# startAnimating()

Begins animating the current sequence of images.

watchOS

``` source
func startAnimating()
```

**Required**

## Discussion

If the image data contains multiple images, calling this method begins animating through those images, starting at the first image. The animation uses the duration value specified in your storyboard file.

If the current image contains only a single image, this method does nothing.

## See Also

### Animating an Image Sequence

func startAnimatingWithImages(in: NSRange, duration: TimeInterval, repeatCount: Int)

Animates the specified images with the given duration and repeat information.

**Required**

func stopAnimating()

Stops any in-progress animations.

**Required**

