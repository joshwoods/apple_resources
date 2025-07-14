

- SceneKit
- SCNCamera
-  focalSize Deprecated

Instance Property

# focalSize

The width of the distance range at which objects appear in sharp focus. Animatable.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var focalSize: CGFloat { get set }
```

Deprecated

Use focusDistance instead; see also fStop.

## Discussion

The focalDistance property specifies how far away from the camera an object needs to be to appear in sharp focus. Focal size specifies how wide an area around that distance also appears in sharp focus. The default focus size is `0.0`, specifying that the transition from sharp to blurred begins for objects immediately nearer to or farther from the camera than the focal distance. When focal size is nonzero, it specifies the distance between the nearest an object can be to the camera and remain in sharp focus to the farthest an object can be from the camera and remain in sharp focus.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Deprecated

var yFov: Double

The camera’s field of view, in degrees, on the vertical axis. Animatable.

Deprecated

var xFov: Double

The camera’s field of view, in degrees, on the horizontal axis. Animatable.

Deprecated

var focalDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

Deprecated

var focalBlurRadius: CGFloat

The maximum amount of blurring, in pixels, applied to areas outside the camera’s depth of field. Animatable.

Deprecated

var aperture: CGFloat

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

Deprecated

