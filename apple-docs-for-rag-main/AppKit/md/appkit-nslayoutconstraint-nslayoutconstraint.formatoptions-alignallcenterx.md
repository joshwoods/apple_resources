

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.FormatOptions
-  alignAllCenterX 

Type Property

# alignAllCenterX

Align all specified interface elements using NSLayoutConstraint.Attribute.centerX on each.

macOS

``` source
static var alignAllCenterX: NSLayoutConstraint.FormatOptions { get }
```

## See Also

### Constants

static var alignAllLeft: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.left on each.

static var alignAllRight: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.right on each.

static var alignAllTop: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.top on each.

static var alignAllBottom: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.bottom on each.

static var alignAllLeading: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.leading on each.

static var alignAllTrailing: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.trailing on each.

static var alignAllCenterY: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.centerY on each.

static var alignAllLastBaseline: NSLayoutConstraint.FormatOptions

Align all specified interface elements using the last baseline of each one.

static var alignAllFirstBaseline: NSLayoutConstraint.FormatOptions

Align all specified interface elements using the first baseline of each one.

static var alignmentMask: NSLayoutConstraint.FormatOptions

Bit mask that can be combined with an NSLayoutConstraint.FormatOptions variable to yield only the alignment portion of the format options.

static var directionLeadingToTrailing: NSLayoutConstraint.FormatOptions

Arrange objects in order based on the normal text flow for the current user interface language. In left-to-right languages (like English), this arrangement results in the first object being placed farthest to the left, the next one to its right, and so on. In right-to-left languages (like Arabic or Hebrew), the ordering is reversed.

static var directionLeftToRight: NSLayoutConstraint.FormatOptions

Arrange objects in order from left to right.

static var directionRightToLeft: NSLayoutConstraint.FormatOptions

Arrange objects in order from right to left.

static var directionMask: NSLayoutConstraint.FormatOptions

A bit mask that can be combined with an NSLayoutConstraint.FormatOptions variable to yield only the direction portion of the format options.

