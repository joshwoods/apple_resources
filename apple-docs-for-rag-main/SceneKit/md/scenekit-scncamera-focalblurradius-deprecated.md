

- SceneKit
- SCNCamera
-  focalBlurRadius Deprecated

Instance Property

# focalBlurRadius

The maximum amount of blurring, in pixels, applied to areas outside the camera’s depth of field. Animatable.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var focalBlurRadius: CGFloat { get set }
```

Deprecated

Use fStop instead to define physically based variable blur effects instead of a constant radius. (Note fStop `=` sensorHeight `/` aperture.)

## Discussion

The default value of this property is `0.0`, disabling the depth of field visual effect. Changing this property to a nonzero value enables the depth of field effect, in which only objects at a specified distance from the camera appear in sharp focus, and objects nearer to or farther from the camera appear increasingly blurred (up to the amount specified by this property).

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

var focalSize: CGFloat

The width of the distance range at which objects appear in sharp focus. Animatable.

Deprecated

var aperture: CGFloat

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

Deprecated

