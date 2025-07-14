

- WebKit
- WebFrameView
-  allowsScrolling Deprecated

Instance Property

# allowsScrolling

A Boolean that indicates whether the frame view should allow users to scroll.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var allowsScrolling: Bool { get set }
```

## Discussion

If true, scrolling is allowed; if false, it is not. If the frame contains a scrolling element, then that value is used as the default; otherwise, the default is true.

