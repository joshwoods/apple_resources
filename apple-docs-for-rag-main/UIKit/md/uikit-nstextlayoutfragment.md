

- UIKit
-  NSTextLayoutFragment 

Class

# NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class NSTextLayoutFragment
```

## Topics

### Creating a layout fragment

init?(coder: NSCoder)

Creates a new layout fragment with the coder you provide.

init(textElement: NSTextElement, range: NSTextRange?)

Create a new layout fragment using the provided text element and range.

### Getting line fragments

var textLineFragments: [NSTextLineFragment]

An array of text line fragments.

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func textLineFragment(for: any NSTextLocation, isUpstreamAffinity: Bool) -> NSTextLineFragment?

Returns a text line fragment from a specific text location in the document.

func textLineFragment(forVerticalOffset: CGFloat, requiresExactMatch: Bool) -> NSTextLineFragment?

Returns the text line fragment for the vertical offset you provide, or the closest text line fragment beyond the vertical offset.

### Getting element information

var state: NSTextLayoutFragment.State

The layout information state.

enum State

Values that describe the possible layout states.

var rangeInElement: NSTextRange

The range inside the text element relative to the document origin.

var textElement: NSTextElement?

The parent text element.

### Accessing the layout manager

var textLayoutManager: NSTextLayoutManager?

The layout manager for this text layout fragment.

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

func frameForTextAttachment(at: any NSTextLocation) -> CGRect

Returns the frame in the text layout fragment coordinate system for the attachment at the location you specify.

### Accessing the layout processing queue

var layoutQueue: OperationQueue?

The queue on which the framework dispatches layout operations.

### Defining margins and padding

var bottomMargin: CGFloat

The amount of space reserved during paragraph layout between the bottom of the last line in the paragraph and the bottom of the text layout fragment.

var leadingPadding: CGFloat

The amount of margin space reserved during paragraph layout between the leading edge of the text layout fragment and the start of the lines in the paragraph.

var topMargin: CGFloat

The amount of space reserved during paragraph layout between the top of the text layout fragment and the top of the first line in the paragraph.

var trailingPadding: CGFloat

The amount of margin space reserved during paragraph layout between the end of the lines in the paragraph and the trailing edge of the text layout fragment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

Display text with a custom layout

Lay out text in a custom-shaped container and apply glyph substitutions.

class NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

class NSTextContainer

A region where text layout occurs.

class NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

class NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

protocol NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

