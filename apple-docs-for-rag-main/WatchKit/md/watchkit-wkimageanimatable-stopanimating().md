

- WatchKit
- WKImageAnimatable
-  stopAnimating() 

Instance Method

# stopAnimating()

Stops any in-progress animations.

watchOS

``` source
func stopAnimating()
```

**Required**

## Discussion

If no animation is in progress, this method does nothing.

## See Also

### Animating an Image Sequence

func startAnimating()

Begins animating the current sequence of images.

**Required**

func startAnimatingWithImages(in: NSRange, duration: TimeInterval, repeatCount: Int)

Animates the specified images with the given duration and repeat information.

**Required**

