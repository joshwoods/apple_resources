

- SceneKit
- SCNView
-  SCNView.Option 

Structure

# SCNView.Option

Dictionary keys specifying initialization options, used when initializing a SceneKit view.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct Option
```

## Topics

### View Options

static let preferLowPowerDevice: SCNView.Option

An option for whether to select low-power-usage devices for Metal rendering.

static let preferredDevice: SCNView.Option

The device to use for Metal rendering.

static let preferredRenderingAPI: SCNView.Option

The rendering API to use for rendering the view (for example, Metal or OpenGL).

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Initializing a SceneKit View

init(frame: CGRect, options: [String : Any]?)

Initializes and returns a newly allocated SceneKit view object with the specified frame rectangle and options.

