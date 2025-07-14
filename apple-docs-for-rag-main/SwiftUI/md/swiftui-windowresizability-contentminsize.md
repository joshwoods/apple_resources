

- SwiftUI
- WindowResizability
-  contentMinSize 

Type Property

# contentMinSize

A window resizability that’s partially derived from the window’s content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
static var contentMinSize: WindowResizability { get set }
```

## Discussion

Windows that use this resizability have:

- A minimum size that matches the minimum size of the window’s content.

- No maximum size.

## See Also

### Getting the resizability

static var automatic: WindowResizability

The automatic window resizability.

static var contentSize: WindowResizability

A window resizability that’s derived from the window’s content.

