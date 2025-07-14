

- SceneKit
- SCNView
- SCNView.Option
-  preferredRenderingAPI 

Type Property

# preferredRenderingAPI

The rendering API to use for rendering the view (for example, Metal or OpenGL).

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+

``` source
static let preferredRenderingAPI: SCNView.Option
```

## Discussion

The value for this key is an NSNumber object containing one of the values listed in SCNRenderingAPI. You can also set this option from the inspector in Interface Builder.

SceneKit attempts to initialize a view using the preferred API you specify in the SCNView initializer; if the current device does not support the preferred API, SceneKit automatically falls back to a supported API. After initialization, use the renderingAPI property to find out whether a fallback occurred. For example, if you specify the SCNRenderingAPI.metal option when initializing a view on an iOS device that does not support Metal, SceneKit defaults to the SCNRenderingAPI.openGLES2 option instead.

## See Also

### View Options

static let preferLowPowerDevice: SCNView.Option

An option for whether to select low-power-usage devices for Metal rendering.

static let preferredDevice: SCNView.Option

The device to use for Metal rendering.

