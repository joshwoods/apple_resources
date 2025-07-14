

- SceneKit
- SCNCamera
-  yFov Deprecated

Instance Property

# yFov

The camera’s field of view, in degrees, on the vertical axis. Animatable.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var yFov: Double { get set }
```

Deprecated

Use fieldOfView instead; see also projectionDirection.

## Discussion

Field of view is an angle that determines the extent of the scene visible to the camera, similar to that of a real-world camera lens. A small field of view angle provides a narrow view, and a large field of view provides a wide view. A very wide field of view results in distorted perspective.

SceneKit allows horizontal and vertical field of view to be set independently. By default, both the xFov and yFov properties are zero, causing SceneKit to use a 60° vertical field of view and automatically adjust the horizontal field of view to fit the renderer’s aspect ratio without distorting the image. If you set only one of the field of view properties to a nonzero value, SceneKit uses that value for its axis and automatically adjusts the field of view in the other axis. If you set both properties, SceneKit uses the property that best fits the renderer’s current aspect ratio and automatically adjusts the field of view in the other axis.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Deprecated

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

var aperture: CGFloat

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

Deprecated

