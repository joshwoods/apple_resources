

- UIKit
- NSTextLayoutFragment
-  draw(at:in:) 

Instance Method

# draw(at:in:)

Renders the visual representation of this element in the specified graphics context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func draw(
    at point: CGPoint,
    in context: CGContext
)
```

## Parameters 

`point`  

The origin as a CGPoint.

`context`  

The rendering context.

## See Also

### Drawing the fragment and attachments

var layoutFragmentFrame: CGRect

The rectangle the framework uses for tiling the layout fragment inside the target layout coordinate system.

var renderingSurfaceBounds: CGRect

The bounds defining the area required for rendering the contents.

func invalidateLayout()

Invalidates any layout information associated with the text layout fragment.

var textAttachmentViewProviders: [NSTextAttachmentViewProvider]

The attachment view provider associated with the text layout fragment.

func frameForTextAttachment(at: any NSTextLocation) -> CGRect

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

