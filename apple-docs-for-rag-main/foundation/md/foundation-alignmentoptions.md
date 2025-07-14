

- Foundation
-  AlignmentOptions 

Structure

# AlignmentOptions

Values representing alignment operations.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AlignmentOptions
```

## Overview

These constants are used by the NSIntegralRectWithOptions(_:_:) function and other related methods, such as backingAlignedRect(_:options:).

## Topics

### Constants

static var alignMinXInward: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest inward integral value.

static var alignMinYInward: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest inward integral value.

static var alignMaxXInward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest inward integral value.

static var alignMaxYInward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest inward integral value.

static var alignWidthInward: AlignmentOptions

Specifies that alignment of the width should be to the nearest inward integral value.

static var alignHeightInward: AlignmentOptions

Specifies that alignment of the height should be to the nearest inward integral value.

static var alignMinXOutward: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest outward integral value.

static var alignMinYOutward: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest outward integral value.

static var alignMaxXOutward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest outward integral value.

static var alignMaxYOutward: AlignmentOptions

Specifies that alignment of the maximum Y coordinate should be to the nearest outward integral value.

static var alignWidthOutward: AlignmentOptions

Specifies that alignment of the width should be to the nearest outward integral value.

static var alignHeightOutward: AlignmentOptions

Specifies that alignment of the height should be to the nearest outward integral value.

static var alignMinXNearest: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest integral value.

static var alignMinYNearest: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest integral value.

static var alignMaxXNearest: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest integral value.

static var alignMaxYNearest: AlignmentOptions

Specifies that alignment of the maximum Y coordinate should be to the nearest integral value.

static var alignWidthNearest: AlignmentOptions

Specifies that alignment of the width should be to the nearest integral value.

static var alignHeightNearest: AlignmentOptions

Specifies that alignment of the height should be to the nearest integral value.

static var alignRectFlipped: AlignmentOptions

This option should be included if the rectangle is in a flipped coordinate system. This allows 0.5 to be treated in a visually consistent way.

static var alignAllEdgesInward: AlignmentOptions

Aligns all edges inward. This is the same as `NSAlignMinXInward|NSAlignMaxXInward|NSAlignMinYInward|NSAlignMaxYInward`.

static var alignAllEdgesOutward: AlignmentOptions

Aligns all edges outwards. This is the same as `NSAlignMinXOutward|NSAlignMaxXOutward|NSAlignMinYOutward|NSAlignMaxYOutward`.

static var alignAllEdgesNearest: AlignmentOptions

Aligns all edges to the nearest value. This is the same as `NSAlignMinXNearest|NSAlignMaxXNearest|NSAlignMinYNearest|NSAlignMaxYNearest`.

static var alignMinXInward: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest inward integral value.

static var alignMinYInward: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest inward integral value.

static var alignMaxXInward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest inward integral value.

static var alignMaxYInward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest inward integral value.

static var alignWidthInward: AlignmentOptions

Specifies that alignment of the width should be to the nearest inward integral value.

static var alignHeightInward: AlignmentOptions

Specifies that alignment of the height should be to the nearest inward integral value.

static var alignMinXOutward: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest outward integral value.

static var alignMinYOutward: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest outward integral value.

static var alignMaxXOutward: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest outward integral value.

static var alignMaxYOutward: AlignmentOptions

Specifies that alignment of the maximum Y coordinate should be to the nearest outward integral value.

static var alignWidthOutward: AlignmentOptions

Specifies that alignment of the width should be to the nearest outward integral value.

static var alignHeightOutward: AlignmentOptions

Specifies that alignment of the height should be to the nearest outward integral value.

static var alignMinXNearest: AlignmentOptions

Specifies that alignment of the minimum X coordinate should be to the nearest integral value.

static var alignMinYNearest: AlignmentOptions

Specifies that alignment of the minimum Y coordinate should be to the nearest integral value.

static var alignMaxXNearest: AlignmentOptions

Specifies that alignment of the maximum X coordinate should be to the nearest integral value.

static var alignMaxYNearest: AlignmentOptions

Specifies that alignment of the maximum Y coordinate should be to the nearest integral value.

static var alignWidthNearest: AlignmentOptions

Specifies that alignment of the width should be to the nearest integral value.

static var alignHeightNearest: AlignmentOptions

Specifies that alignment of the height should be to the nearest integral value.

static var alignRectFlipped: AlignmentOptions

This option should be included if the rectangle is in a flipped coordinate system. This allows 0.5 to be treated in a visually consistent way.

static var alignAllEdgesInward: AlignmentOptions

Aligns all edges inward. This is the same as `NSAlignMinXInward|NSAlignMaxXInward|NSAlignMinYInward|NSAlignMaxYInward`.

static var alignAllEdgesOutward: AlignmentOptions

Aligns all edges outwards. This is the same as `NSAlignMinXOutward|NSAlignMaxXOutward|NSAlignMinYOutward|NSAlignMaxYOutward`.

static var alignAllEdgesNearest: AlignmentOptions

Aligns all edges to the nearest value. This is the same as `NSAlignMinXNearest|NSAlignMaxXNearest|NSAlignMinYNearest|NSAlignMaxYNearest`.

### Initializers

init(rawValue: UInt64)

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

### Related Types

enum NSRectEdge

typealias NSRectArray

Type indicating a parameter is array of `NSRect` structures.

typealias NSRectPointer

Type indicating a parameter is a pointer to an `NSRect` structure.

