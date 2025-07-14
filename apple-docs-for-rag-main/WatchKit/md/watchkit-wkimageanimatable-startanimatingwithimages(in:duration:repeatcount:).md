

- WatchKit
- WKImageAnimatable
-  startAnimatingWithImages(in:duration:repeatCount:) 

Instance Method

# startAnimatingWithImages(in:duration:repeatCount:)

Animates the specified images with the given duration and repeat information.

watchOS

``` source
func startAnimatingWithImages(
    in imageRange: NSRange,
    duration: TimeInterval,
    repeatCount: Int
)
```

**Required**

## Parameters 

`imageRange`  

The range of images to be animated. The value `0` indicates the first image in the sequence, the value `1` the second image, and so on.

`duration`  

The time (in seconds) over which to animate a single loop of the images. Positive values cause the animation to start at the first frame in the sequence and end on the last frame. Negative values causes the animation to play in reverse order and end on the first frame in the sequence.

`repeatCount`  

The number of times to repeat the animation loop. Specify `0` to animate the images indefinitely.

## Discussion

This method animates a subset of the images associated with the current image interface object. This method starts the animation from the first image in the specified range.

## See Also

### Animating an Image Sequence

func startAnimating()

Begins animating the current sequence of images.

**Required**

func stopAnimating()

Stops any in-progress animations.

**Required**

