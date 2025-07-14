

- AppKit
- NSTextLayoutManager
-  enumerateTextLayoutFragments(from:options:using:) 

Instance Method

# enumerateTextLayoutFragments(from:options:using:)

Enumerates the text layout fragments starting at the specified location.

macOS 12.0+

``` source
func enumerateTextLayoutFragments(
    from location: (any NSTextLocation)?,
    options: NSTextLayoutFragment.EnumerationOptions = [],
    using block: (NSTextLayoutFragment) -> Bool
) -> (any NSTextLocation)?
```

## Parameters 

`location`  

The location where youstart the enumeration.

`options`  

One or more of the available NSTextLayoutFragment.EnumerationOptions.

`block`  

A closure you provide that determines if the enumeration finishes early.

## Return Value

An NSTextLocation, or `nil`.

## Discussion

If `textLocation` is `nil`, the method starts at `self.textContentManager.documentRange.location`.The method uses `self.documentRange.endLocation` for reverse enumeration. When enumerating backward, it starts with the fragment preceding the one containing `textLocation`. If the method enumerates at least one fragment, it returns the edge of the enumerated range.

The enumerated range might not match the range of the last element returned; it enumerates the elements in the sequence, but it can skip a range. For example, it can limit the maximum number of text elements the method enumerates for a single invocation or hide some elements from the layout.

Returning `false` from `block` breaks out of the enumeration.

## See Also

### Causing layout generation

var textViewportLayoutController: NSTextViewportLayoutController

Returns text viewport layout controller associated with the layout manager’s text container.

func invalidateLayout(for: NSTextRange)

Invalidates the layout information for specified text range.

func textLayoutFragment(for: any NSTextLocation) -> NSTextLayoutFragment?

Returns the text layout fragment from the document at the specified location.

func textLayoutFragment(for: CGPoint) -> NSTextLayoutFragment?

Returns the text layout fragment at the position you specify in the text container.

func ensureLayout(for: CGRect)

Performs the layout for filling the bounds you specify inside the last text container.

func ensureLayout(for: NSTextRange)

Performs the layout for specified text range.

enum SegmentType

Values that describe the rendering of selection boundaries.

struct SegmentOptions

Values that describe where and how the framework extends segments of a selection.

