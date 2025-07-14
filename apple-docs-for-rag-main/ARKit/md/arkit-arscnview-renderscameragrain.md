

- ARKit
- ARSCNView
-  rendersCameraGrain 

Instance Property

# rendersCameraGrain

A flag that determines whether SceneKit applies image noise characteristics to your app’s virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var rendersCameraGrain: Bool { get set }
```

## Discussion

Enabled by default. When set, SceneKit adds a camera grain effect to your app’s virtual content that matches the image noise characteristics ARKit observes in the camera feed.

## See Also

### Managing Rendering Effects

var rendersMotionBlur: Bool

Determines whether the view renders motion blur.

