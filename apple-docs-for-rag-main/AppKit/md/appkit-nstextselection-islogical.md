

- AppKit
- NSTextSelection
-  isLogical 

Instance Property

# isLogical

A Boolean value that indicates whether the framework interprets the selection as logical or visual.

macOS 12.0+

``` source
var isLogical: Bool { get set }
```

## See Also

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

