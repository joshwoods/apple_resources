

- AppKit
- NSTextLayoutFragment
-  layoutFragmentFrame 

Instance Property

# layoutFragmentFrame

The rectangle the framework uses for tiling the layout fragment inside the target layout coordinate system.

macOS 12.0+

``` source
var layoutFragmentFrame: CGRect { get }
```

## See Also

### Drawing the fragment and attachments

var renderingSurfaceBounds: CGRect

The bounds defining the area required for rendering the contents.

func draw(at: CGPoint, in: CGContext)

Renders the visual representation of this element in the specified graphics context.

func invalidateLayout()

Invalidates any layout information associated with the text layout fragment.

var textAttachmentViewProviders: [NSTextAttachmentViewProvider]

The attachment view provider associated with the text layout fragment.

func frameForTextAttachment(at: any NSTextLocation) -> CGRect

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

