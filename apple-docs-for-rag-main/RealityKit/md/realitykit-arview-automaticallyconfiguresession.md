

- RealityKit
- ARView
-  automaticallyConfigureSession 

Instance Property

# automaticallyConfigureSession

An indication of whether to use an automatically configured AR session.

iOSiPadOSMac Catalyst

``` source
@MainActor @preconcurrency
var automaticallyConfigureSession: Bool { get set }
```

## Discussion

When enabled, the ARView automatically runs an `RealityKit/ARSession` with a default configuration. RealityKit updates that configuration based on t camera mode and scene anchors. When disabled, you need to provide a configuration object and run the session manually.

The default value is true.

## See Also

### Configuring the AR session

var session: ARSession

The AR session that supports the view’s rendering.

var renderOptions: ARView.RenderOptions

The render options that configure the view’s AR session.

var renderCallbacks: ARView.RenderCallbacks

A container that holds the view’s render callbacks.

