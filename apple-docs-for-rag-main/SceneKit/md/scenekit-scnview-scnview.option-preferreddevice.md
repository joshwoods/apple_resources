

- SceneKit
- SCNView
- SCNView.Option
-  preferredDevice 

Type Property

# preferredDevice

The device to use for Metal rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static let preferredDevice: SCNView.Option
```

## Discussion

The value for this key is a MTLDevice object.

Use this key to choose a specific device for rendering (for example, on a macOS system with multiple GPUs), or leave it unspecified to allow SceneKit to automatically choose a device.

## See Also

### View Options

static let preferLowPowerDevice: SCNView.Option

An option for whether to select low-power-usage devices for Metal rendering.

static let preferredRenderingAPI: SCNView.Option

The rendering API to use for rendering the view (for example, Metal or OpenGL).

