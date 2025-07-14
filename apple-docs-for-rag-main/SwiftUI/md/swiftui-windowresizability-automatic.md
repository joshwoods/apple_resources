

- SwiftUI
- WindowResizability
-  automatic 

Type Property

# automatic

The automatic window resizability.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
static var automatic: WindowResizability { get set }
```

## Discussion

When you use automatic resizability, SwiftUI applies a resizing strategy that’s appropriate for the scene type:

- Windows from WindowGroup, Window, and DocumentGroup scene declarations use the contentMinSize strategy.

- A window from a Settings scene declaration uses the contentSize strategy.

- Windows on visionOS with a window style of volumetric use the contentSize strategy.

Automatic resizability is the default if you don’t specify another value using the windowResizability(_:) scene modifier.

## See Also

### Getting the resizability

static var contentMinSize: WindowResizability

A window resizability that’s partially derived from the window’s content.

static var contentSize: WindowResizability

A window resizability that’s derived from the window’s content.

