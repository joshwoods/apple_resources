

- RealityKit
- ARView
-  renderOptions 

Instance Property

# renderOptions

The render options that configure the view’s AR session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
@MainActor @preconcurrency
var renderOptions: ARView.RenderOptions { get set }
```

## Mentioned in 

Reducing GPU Utilization in Your RealityKit App

## Discussion

RealityKit applies effects like camera grain, motion blur, and depth of field to the render to make the AR experience more immersive. Each effect causes your virtual content to better blend in with live images from the camera in some way.

To disable an effect, you add an option from the ARView.RenderOptions option set to the view’s renderOptions property:

```
arView.renderOptions.insert(.disableMotionBlur) // Turn off motion blur.
```

When you create an AR view, the system automatically adds certain render options to disable effects that might be too demanding for the GPU hardware on which your app is running. But you can modify the renderOptions set at any time to enable or disable any particular effect, depending on the needs of your app.

To decide whether to use an effect, consider both its visual impact on your app, and its computational cost. Check the cost by measuring your app’s CPU and GPU utilization with the effect enabled across all the devices your app supports, as described in Improving the Performance of a RealityKit App.

## See Also

### Configuring the AR session

var session: ARSession

The AR session that supports the view’s rendering.

var automaticallyConfigureSession: Bool

An indication of whether to use an automatically configured AR session.

var renderCallbacks: ARView.RenderCallbacks

A container that holds the view’s render callbacks.

