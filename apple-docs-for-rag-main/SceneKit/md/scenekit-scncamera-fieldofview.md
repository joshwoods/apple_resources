

- SceneKit
- SCNCamera
-  fieldOfView 

Instance Property

# fieldOfView

The vertical or horizontal viewing angle of the camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var fieldOfView: CGFloat { get set }
```

## Discussion

The projectionDirection property determines whether this fieldOfView property measures the camera’s vertical or horizontal viewing angle, and SceneKit automatically calculates the viewing angle in the other direction to match the aspect ratio of the view displaying the scene. For example, a fieldOfView of `60` and the default SCNCameraProjectionDirection.vertical projection, presented fullscreen on a 16:9 display in portrait orientation, results in a vertical viewing angle of 60° and a horizontal viewing angle of 33.75°.

You can choose to specify viewing angle either directly, using this fieldOfView property, or in terms that model a physical camera, using the sensorHeight and focalLength properties. Setting the fieldOfView property causes SceneKit to automatically recalculate the focalLength value, and setting the sensorHeight or focalLength property recalculates fieldOfView.

## See Also

### Managing Field of View

var focalLength: CGFloat

The camera’s focal length, in millimeters.

var sensorHeight: CGFloat

The vertical size of the camera’s imaging plane, in millimeters.

var projectionDirection: SCNCameraProjectionDirection

The axis used to determine field of view or orthographic scale.

enum SCNCameraProjectionDirection

Options for the axis used to determine field of view or orthographic projection.

