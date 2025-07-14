

- SwiftUI
- Anchor
- Anchor.Source
-  rect(\_:) 

Type Method

# rect(\_:)

Returns an anchor source rect defined by `r` in the current view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func rect(_ r: CGRect) -> Anchor.Source
```

Available when `Value` is `CGRect`.

## See Also

### Getting rectangle anchor sources

static var bounds: Anchor&lt;CGRect>.Source

An anchor source rect defined as the entire bounding rect of the current view.

