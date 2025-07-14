

- SwiftUI
- ImageRenderer
-  nsImage 

Instance Property

# nsImage

The current contents of the view, rasterized as an AppKit image.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
@MainActor
final var nsImage: NSImage? { get }
```

Available when `Content` conforms to `View`.

## Discussion

The renderer notifies its `objectWillChange` publisher when the contents of the image may have changed.

## See Also

### Rendering images

func render(rasterizationScale: CGFloat, renderer: (CGSize, (CGContext) -> Void) -> Void)

Draws the renderer’s current contents to an arbitrary Core Graphics context.

var cgImage: CGImage?

The current contents of the view, rasterized as a Core Graphics image.

var uiImage: UIImage?

The current contents of the view, rasterized as a UIKit image.

