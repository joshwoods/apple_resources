

- SceneKit
- SCNCamera
-  focalLength 

Instance Property

# focalLength

The camera’s focal length, in millimeters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var focalLength: CGFloat { get set }
```

## Discussion

The sensorHeight and focalLength properties determine the camera’s horizontal and vertical viewing angles using terms that model physical camera devices. (Alternatively, you can work with viewing angle directly though the fieldOfView property.) For example, with the default sensor height of 24 mm and default focal length of 50 mm, the vertical field of view is 60°.

Setting the fieldOfView property causes SceneKit to automatically recalculate the focalLength value, and setting the sensorHeight or focalLength property recalculates fieldOfView.

## See Also

### Managing Field of View

var fieldOfView: CGFloat

The vertical or horizontal viewing angle of the camera.

var sensorHeight: CGFloat

The vertical size of the camera’s imaging plane, in millimeters.

var projectionDirection: SCNCameraProjectionDirection

The axis used to determine field of view or orthographic scale.

enum SCNCameraProjectionDirection

Options for the axis used to determine field of view or orthographic projection.

