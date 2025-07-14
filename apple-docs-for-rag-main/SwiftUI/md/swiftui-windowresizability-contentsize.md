

- SwiftUI
- WindowResizability
-  contentSize 

Type Property

# contentSize

A window resizability that’s derived from the window’s content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
static var contentSize: WindowResizability { get set }
```

## Discussion

Windows that use this resizability have:

- A minimum size that matches the minimum size of the window’s content.

- A maximum size that matches the maximum size of the window’s content.

## See Also

### Getting the resizability

static var automatic: WindowResizability

The automatic window resizability.

static var contentMinSize: WindowResizability

A window resizability that’s partially derived from the window’s content.

