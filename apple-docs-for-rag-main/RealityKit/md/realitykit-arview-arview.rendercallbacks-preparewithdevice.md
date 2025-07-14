

- RealityKit
- ARView
- ARView.RenderCallbacks
-  prepareWithDevice 

Instance Property

# prepareWithDevice

A callback function for doing initial setup work.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var prepareWithDevice: ((any MTLDevice) -> Void)?
```

## Mentioned in 

Applying core image filters as a postprocess effect

Implementing postprocess effects using Metal compute functions

## Discussion

If you assign a function to prepareWithDevice, RealityKit calls that function once, after it does its setup work, but before it renders the next frame. If you register a prepareWithDevice callback during app startup, RealityKit calls it before it renders the first frame. A callback function looks like this:

```
    func myPostProcessSetupCallback(device: MTLDevice) {
        // Handle setup work here.
    }
```

To register the function so RealityKit calls it, assign it to the prepareWithDevice property of the view’s renderCallbacks property.

```
arView.renderCallbacks.prepareWithDevice = myPostProcessSetupCallback
```

To remove the callback, assign `nil`.

```
arView.renderCallbacks.prepareWithDevice = nil
```

If you assign a new closure or function to the property after setting it to `nil`, RealityKit calls the new closure before it renders the next frame. In that case, avoid doing long-running tasks in the callback function to avoid rendering hitches.

## See Also

### Register callback closures

var postProcess: ((ARView.PostProcessContext) -> Void)?

A callback function for implementing postprocess effects.

