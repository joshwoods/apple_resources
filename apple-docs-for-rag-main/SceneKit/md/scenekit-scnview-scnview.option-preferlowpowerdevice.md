

- SceneKit
- SCNView
- SCNView.Option
-  preferLowPowerDevice 

Type Property

# preferLowPowerDevice

An option for whether to select low-power-usage devices for Metal rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static let preferLowPowerDevice: SCNView.Option
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value.

SceneKit uses this option when automatically selecting a Metal device on systems with multiple GPUs. If the value is true, SceneKit uses a device with low power usage requirements—for example, the integrated GPU on a MacBook Pro with both integrated and discrete graphics hardware.

Leaving this key unspecified is equivalent to setting its value to false. In this case, SceneKit chooses the most capable available Metal device.

## See Also

### View Options

static let preferredDevice: SCNView.Option

The device to use for Metal rendering.

static let preferredRenderingAPI: SCNView.Option

The rendering API to use for rendering the view (for example, Metal or OpenGL).

