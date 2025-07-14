

- AVKit
- AVPlayerView
-  setMagnification(\_:centeredAt:) 

Instance Method

# setMagnification(\_:centeredAt:)

Scales the video’s view by a specified factor, and centers the result on a specified point.

macOS 13.0+

``` source
@MainActor
func setMagnification(
    _ magnification: CGFloat,
    centeredAt point: CGPoint
)
```

## Parameters 

`magnification`  

A factor by which to scale the video’s view.

`point`  

A point in view space on which to center magnification.

## Discussion

The supported magnification range is `1.0` to `64.0`. The system zooms using nearest neighbor interpolation after it scales the content past a certain factor.

## See Also

### Magnifying Video

var allowsMagnification: Bool

A Boolean value that indicates whether the magnify gesture changes the video’s view magnification.

var magnification: CGFloat

The factor by which the video’s view is currently scaled.

