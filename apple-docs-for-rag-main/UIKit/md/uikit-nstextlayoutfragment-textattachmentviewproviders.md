

- UIKit
- NSTextLayoutFragment
-  textAttachmentViewProviders 

Instance Property

# textAttachmentViewProviders

The attachment view provider associated with the text layout fragment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var textAttachmentViewProviders: [NSTextAttachmentViewProvider] { get }
```

## Discussion

The property contents are only valid with NSTextLayoutFragment.State.layoutAvailable.

## See Also

### Drawing the fragment and attachments

var layoutFragmentFrame: CGRect

The rectangle the framework uses for tiling the layout fragment inside the target layout coordinate system.

var renderingSurfaceBounds: CGRect

The bounds defining the area required for rendering the contents.

func draw(at: CGPoint, in: CGContext)

Renders the visual representation of this element in the specified graphics context.

func invalidateLayout()

Invalidates any layout information associated with the text layout fragment.

func frameForTextAttachment(at: any NSTextLocation) -> CGRect

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

