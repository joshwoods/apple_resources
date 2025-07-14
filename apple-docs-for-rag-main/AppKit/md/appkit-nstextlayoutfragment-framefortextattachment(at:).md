

- AppKit
- NSTextLayoutFragment
-  frameForTextAttachment(at:) 

Instance Method

# frameForTextAttachment(at:)

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

macOS 12.0+

``` source
func frameForTextAttachment(at location: any NSTextLocation) -> CGRect
```

## Parameters 

`location`  

The NSTextLocation that describes the location in the text layout fragment.

## Return Value

The frame rectangle that describes the text layout fragment.

## Discussion

Returns CGRectZero if `location` isn’t with any attachment or the state isn’t NSTextLayoutFragment.State.layoutAvailable.

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

var textAttachmentViewProviders: [NSTextAttachmentViewProvider]

The attachment view provider associated with the text layout fragment.

