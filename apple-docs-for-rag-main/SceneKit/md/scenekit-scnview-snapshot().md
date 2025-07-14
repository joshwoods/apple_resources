

- SceneKit
- SCNView
-  snapshot() 

Instance Method

# snapshot()

Renders the view’s scene into a new image object.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

**macOS**

``` source
@MainActor
func snapshot() -> NSImage
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func snapshot() -> UIImage
```

## Return Value

An image object depicting the view in its current state.

## Discussion

This method is thread-safe and may be called at any time.

