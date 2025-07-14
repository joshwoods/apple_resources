

- UIKit
- NSTextLayoutManager
-  NSTextLayoutManager.SegmentOptions 

Structure

# NSTextLayoutManager.SegmentOptions

Values that describe where and how the framework extends segments of a selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
struct SegmentOptions
```

## Topics

### Creating segment options

init(rawValue: UInt)

Cceates a new segment option using the value you provide.

### Getting segment options

static var headSegmentExtended: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to extend the segment to the tail edge.

static var middleFragmentsExcluded: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to enumerate segments in only the first and last line fragments.

static var rangeNotRequired: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework enumerate text segment rectangles, but avoids preparing a range object.

static var tailSegmentExtended: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to extend the segment to the tail edge.

static var upstreamAffinity: NSTextLayoutManager.SegmentOptions

Returns the value that causes the framework to the place the segment based on the upstream affinity for an empty range.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

func enumerateTextLayoutFragments(from: (any NSTextLocation)?, options: NSTextLayoutFragment.EnumerationOptions, using: (NSTextLayoutFragment) -> Bool) -> (any NSTextLocation)?

Enumerates the text layout fragments starting at the specified location.

enum SegmentType

Values that describe the rendering of selection boundaries.

