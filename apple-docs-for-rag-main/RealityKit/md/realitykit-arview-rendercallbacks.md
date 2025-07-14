

- RealityKit
- ARView
-  renderCallbacks 

Instance Property

# renderCallbacks

A container that holds the view’s render callbacks.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@MainActor @preconcurrency
var renderCallbacks: ARView.RenderCallbacks { get set }
```

## Mentioned in 

Implementing postprocess effects using Metal compute functions

Applying core image filters as a postprocess effect

## Discussion

Render callbacks are closures RealityKit calls at predefined times. You can use render callbacks to modify the results of RealityKit’s rendering. If you assign a function or closure to any of the contained callback properties, RealityKit calls that function or closure at a predefined time. Setting the `ARView/RenderCallbacks-swift.postProcess` property, for example, causes RealityKit to call the assigned function or closure every frame, after RealityKit renders the scene, but before it displays it.

## See Also

### Configuring the AR session

var session: ARSession

The AR session that supports the view’s rendering.

var automaticallyConfigureSession: Bool

An indication of whether to use an automatically configured AR session.

var renderOptions: ARView.RenderOptions

The render options that configure the view’s AR session.

