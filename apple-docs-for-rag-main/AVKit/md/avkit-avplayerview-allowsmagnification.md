

- AVKit
- AVPlayerView
-  allowsMagnification 

Instance Property

# allowsMagnification

A Boolean value that indicates whether the magnify gesture changes the video’s view magnification.

macOS 13.0+

``` source
@MainActor
var allowsMagnification: Bool { get set }
```

## Discussion

The default value is false. This property only affects whether the magnify gesture triggers magnification. Your app can still programmatically change magnification even when the value of this is false, which matches the behavior of NSScrollView.

## See Also

### Magnifying Video

var magnification: CGFloat

The factor by which the video’s view is currently scaled.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the video’s view by a specified factor, and centers the result on a specified point.

