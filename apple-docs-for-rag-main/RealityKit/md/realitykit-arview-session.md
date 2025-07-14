

- RealityKit
- ARView
-  session 

Instance Property

# session

The AR session that supports the view’s rendering.

iOSiPadOSMac Catalyst

``` source
@MainActor @preconcurrency
dynamic var session: ARSession { get set }
```

## Discussion

RealityKit automatically creates a default session that the view manages. If you have an existing or custom session, setting it as the view’s session replaces the default session. If you replace the default session, you need to start it by calling run(_:options:). See automaticallyConfigureSession for more details.

When automaticallyConfigureSession is true, the default value is an ARWorldTrackingConfiguration.

## See Also

### Configuring the AR session

var automaticallyConfigureSession: Bool

An indication of whether to use an automatically configured AR session.

var renderOptions: ARView.RenderOptions

The render options that configure the view’s AR session.

var renderCallbacks: ARView.RenderCallbacks

A container that holds the view’s render callbacks.

