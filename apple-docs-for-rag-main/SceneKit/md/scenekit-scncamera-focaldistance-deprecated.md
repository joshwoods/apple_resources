

- SceneKit
- SCNCamera
-  focalDistance Deprecated

Instance Property

# focalDistance

The distance from the camera at which objects appear in sharp focus. Animatable.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var focalDistance: CGFloat { get set }
```

Deprecated

Use focusDistance instead.

## Discussion

Objects at this distance from the camera appear perfectly focused. Objects nearer to or farther from the camera than this distance appear increasingly blurred (up to the amount of blur specified by the focalBlurRadius property). The default focal distance is `10.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Deprecated

var yFov: Double

The camera’s field of view, in degrees, on the vertical axis. Animatable.

Deprecated

var xFov: Double

The camera’s field of view, in degrees, on the horizontal axis. Animatable.

Deprecated

var focalSize: CGFloat

The width of the distance range at which objects appear in sharp focus. Animatable.

Deprecated

var focalBlurRadius: CGFloat

The maximum amount of blurring, in pixels, applied to areas outside the camera’s depth of field. Animatable.

Deprecated

var aperture: CGFloat

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

Deprecated

