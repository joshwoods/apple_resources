

- SceneKit
- SCNView
-  init(frame:options:) 

Initializer

# init(frame:options:)

Initializes and returns a newly allocated SceneKit view object with the specified frame rectangle and options.

iOSiPadOSMac CatalystmacOStvOSvisionOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
init(
    frame: CGRect,
    options: [String : Any]? = nil
)
```

**macOS**

``` source
@MainActor
init(
    frame: NSRect,
    options: [String : Any]? = nil
)
```

## Parameters 

`frame`  

The frame rectangle for the view, measured in points and specified in the coordinate system of its superview.

`options`  

Rendering options for the view. See SCNView.

## Return Value

An initialized view object, or `nil` if the object couldn’t be created.

## See Also

### Initializing a SceneKit View

struct Option

Dictionary keys specifying initialization options, used when initializing a SceneKit view.

