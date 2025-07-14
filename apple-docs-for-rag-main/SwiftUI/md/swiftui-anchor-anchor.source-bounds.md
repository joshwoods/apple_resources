

- SwiftUI
- Anchor
- Anchor.Source
-  bounds 

Type Property

# bounds

An anchor source rect defined as the entire bounding rect of the current view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var bounds: Anchor.Source { get }
```

Available when `Value` is `CGRect`.

## See Also

### Getting rectangle anchor sources

static func rect(CGRect) -> Anchor&lt;Value>.Source

Returns an anchor source rect defined by `r` in the current view.

