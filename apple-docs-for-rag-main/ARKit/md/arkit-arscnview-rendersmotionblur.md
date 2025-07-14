

- ARKit
- ARSCNView
-  rendersMotionBlur 

Instance Property

# rendersMotionBlur

Determines whether the view renders motion blur.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var rendersMotionBlur: Bool { get set }
```

## Discussion

This property is enabled by default. When set, the view automatically adds motion blur to rendered content which matches the visual characteristics of the motion blur ARKit observes in the camera feed.

The value of this property overwrites the motionBlurIntensity of SCNCamera.

## See Also

### Managing Rendering Effects

var rendersCameraGrain: Bool

A flag that determines whether SceneKit applies image noise characteristics to your app’s virtual content.

