

- SwiftUI
- ImageRenderer
-  proposedSize 

Instance Property

# proposedSize

The size proposed to the root view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor
final var proposedSize: ProposedViewSize { get set }
```

## Discussion

The default value of this property, unspecified, produces an image that matches the original view size. You can provide a custom ProposedViewSize to override the view’s size in one or both dimensions.

## See Also

### Accessing renderer properties

var scale: CGFloat

The scale at which to render the image.

var isOpaque: Bool

A Boolean value that indicates whether the alpha channel of the image is fully opaque.

var colorMode: ColorRenderingMode

The working color space and storage format of the image.

