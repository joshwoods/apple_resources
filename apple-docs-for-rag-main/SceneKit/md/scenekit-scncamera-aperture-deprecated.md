

- SceneKit
- SCNCamera
-  aperture Deprecated

Instance Property

# aperture

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var aperture: CGFloat { get set }
```

Deprecated

Use fStop instead. Note fStop `=` sensorHeight `/` aperture.

## Discussion

Objects at distances from the camera outside its depth of field (specified by the focalDistance and focalSize properties) appear increasingly blurred (up to the value of the focalBlurRadius property). Aperture controls the abruptness of the transition between sharp and blurred—a low value specifies an abrupt transition, and a higher value specifies a gradual transition. The default aperture is `0.125` (or 1/8).

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

var focalBlurRadius: CGFloat

The maximum amount of blurring, in pixels, applied to areas outside the camera’s depth of field. Animatable.

Deprecated

