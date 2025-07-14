

- AVKit
- AVPlayerView
-  magnification 

Instance Property

# magnification

The factor by which the video’s view is currently scaled.

macOS 13.0+

``` source
@MainActor
var magnification: CGFloat { get set }
```

## Discussion

The supported magnification range is `1.0` to `64.0`. The system zooms using nearest neighbor interpolation after it scales the content past a certain factor.

The default value is `1.0`.

## See Also

### Magnifying Video

var allowsMagnification: Bool

A Boolean value that indicates whether the magnify gesture changes the video’s view magnification.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the video’s view by a specified factor, and centers the result on a specified point.

