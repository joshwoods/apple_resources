

- UIKit
-  NSTextSelection 

Class

# NSTextSelection

A class that represents a single logical selection context that corresponds to an insertion point.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class NSTextSelection
```

## Topics

### Creating a text selection

convenience init(any NSTextLocation, affinity: NSTextSelection.Affinity)

Creates a new text selection with the location and selection affinity you provide.

convenience init(range: NSTextRange, affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the range, selection affinity, and granularity you provide.

init([NSTextRange], affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the ranges, selection affinity, and granularity you provide.

init?(coder: NSCoder)

Creates a test selection from data in an unarchiver.

### Characteristics of a selection

var affinity: NSTextSelection.Affinity

Returns the selection affinity of the text selection.

enum Affinity

Values that describe the visual location of the text cursor, or the direction of the non-anchored edge of the selection.

var anchorPositionOffset: CGFloat

Represents the anchor position offset from the beginning of a line fragment in the visual order for the initial tap or click location.

var granularity: NSTextSelection.Granularity

The granularity of the selection.

enum Granularity

Values that describe the different granularities available to make a selection.

var isLogical: Bool

A Boolean value that indicates whether the framework interprets the selection as logical or visual.

var isTransient: Bool

A Boolean value that indicates transient text selection during drag handling.

var secondarySelectionLocation: (any NSTextLocation)?

Specifies the secondary character location when user taps or clicks at a directional boundary.

protocol NSTextLocation

An interface you implement that represents an abstract location inside your document’s content.

var textRanges: [NSTextRange]

Represents an array of noncontiguous logical ranges in the selection.

var typingAttributes: [NSAttributedString.Key : Any]

The template attributes the framework uses for characters that replace the contents of this selection.

### Creating subselections

func textSelection([NSTextRange]) -> NSTextSelection

Creates a subselection of the current text selection with the ranges you specify.

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

### Location and selection

class NSTextRange

A class that represents a contiguous range between two locations inside document contents.

class NSTextSelectionNavigation

An interface you use to expose methods for obtaining results from actions performed on text selections.

protocol NSTextLocation

An interface you implement that represents an abstract location inside your document’s content.

