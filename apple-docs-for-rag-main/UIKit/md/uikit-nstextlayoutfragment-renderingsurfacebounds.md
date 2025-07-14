

- UIKit
- NSTextLayoutFragment
-  renderingSurfaceBounds 

Instance Property

# renderingSurfaceBounds

The bounds defining the area required for rendering the contents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var renderingSurfaceBounds: CGRect { get }
```

## Discussion

The coordinate system is vertically flipped from the `layoutFragmentFrame` origin ({`0`,`0`} is at the upper-left corner). The size should be larger than `layoutFragmentFrame.size`. The origin could be in the negative coordinate since the rendering could stretch out of `layoutFragmentFrame`. Only valid when `state` greater than NSTextLayoutFragment.State.estimatedUsageBounds.

## See Also

### Drawing the fragment and attachments

var layoutFragmentFrame: CGRect

The rectangle the framework uses for tiling the layout fragment inside the target layout coordinate system.

func draw(at: CGPoint, in: CGContext)

Renders the visual representation of this element in the specified graphics context.

func invalidateLayout()

Invalidates any layout information associated with the text layout fragment.

var textAttachmentViewProviders: [NSTextAttachmentViewProvider]

The attachment view provider associated with the text layout fragment.

func frameForTextAttachment(at: any NSTextLocation) -> CGRect

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

