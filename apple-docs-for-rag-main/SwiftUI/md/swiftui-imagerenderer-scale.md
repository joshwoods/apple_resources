

- SwiftUI
- ImageRenderer
-  scale 

Instance Property

# scale

The scale at which to render the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor
final var scale: CGFloat { get set }
```

## Discussion

This value is a ratio of view points to image pixels. This relationship means that values greater than `1.0` create an image larger than the original content view, and less than `1.0` creates a smaller image. The following example shows a 100 x 50 rectangle view and an image rendered from it with a `scale` of `2.0`, resulting in an image size of 200 x 100.

```
let rectangle = Rectangle()
    .frame(width: 100, height: 50)
let renderer = ImageRenderer(content: rectangle)
renderer.scale = 2.0
if let rendered = renderer.cgImage {
    print("Scaled image: \(rendered.width) x \(rendered.height)")
}
// Prints "Scaled image: 200 x 100"
```

The default value of this property is `1.0`.

## See Also

### Accessing renderer properties

var proposedSize: ProposedViewSize

The size proposed to the root view.

var isOpaque: Bool

A Boolean value that indicates whether the alpha channel of the image is fully opaque.

var colorMode: ColorRenderingMode

The working color space and storage format of the image.

