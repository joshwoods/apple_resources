

- AppKit
- Deprecated Symbols
- NSAccessibility
-  Text-Specific Parameterized Attributes 

API Collection

# Text-Specific Parameterized Attributes

Parameterized attributes specific to text.

## Topics

### Constants

static let lineForIndex: NSAccessibility.ParameterizedAttribute

The line number (`NSNumber`) of the specified character (`NSNumber`).

Deprecated

static let rangeForLine: NSAccessibility.ParameterizedAttribute

The range of characters (`NSValue` containing an `NSRange` value) corresponding to the specified line number (`NSNumber`).

static let stringForRange: NSAccessibility.ParameterizedAttribute

The substring (`NSString`) specified by the range (`NSValue` containing an `NSRange` value).

static let rangeForPosition: NSAccessibility.ParameterizedAttribute

The range of characters (`NSValue` containing an `NSRange` value) composing the glyph at the specified point (`NSValue` containing an `NSPoint` value).

static let rangeForIndex: NSAccessibility.ParameterizedAttribute

The full range of characters (`NSValue` containing an `NSRange` value), including the specified character, which compose a single glyph (`NSNumber`).

static let boundsForRange: NSAccessibility.ParameterizedAttribute

The rectangle (`NSValue` containing an `NSRect` value) enclosing the specified range of characters (`NSValue` containing an `NSRange` value). If the range crosses a line boundary, the returned rectangle will fully enclose all the lines of characters.

static let rtfForRange: NSAccessibility.ParameterizedAttribute

The RTF data (`NSData`) describing the specified range of characters (`NSValue` containing an `NSRange` value).

static let styleRangeForIndex: NSAccessibility.ParameterizedAttribute

The full range of characters (`NSValue` containing an `NSRange` value), including the specified character (`NSNumber`), which have the same style.

static let attributedStringForRange: NSAccessibility.ParameterizedAttribute

Does not use attributes from Appkit/AttributedString.h (`NSAttributedString`).

## See Also

### Constants

Standard Attributes

Standard attributes that can be adopted by any accessibility object.

Text-Specific Attributes

Attributes that are specific to text.

Text Attributed-String Attributes and Constants

Attributes and key constants used with attributed strings.

Window-Specific Attributes

Attributes specific to windows.

App-Specific Attributes

Attributes that are specific to the app object.

Grid View Attributes

Attributes that are used with grid views, such as thumbnails and media browsers that present a grid of items. The children of a grid are ordered.

Table View and Outline View Attributes

Attributes that are specific to tables and outlines.

Outline View Attributes

Attributes that are used in outline views.

Cell-Based Table Attributes

Attributes that are specific to cell-based tables.

Cell-Based Table Parameterized Attributes

Parameterized attributes specific to cell-based tables.

Cell Attributes

Attributes that are specific to individual table cells.

Layout Area Attributes

Attributes that are specific to layout areas.

Layout Area Parameterized Attributes

Parameterized attributes that are specific to layout areas.

Layout Item Attributes

Attributes that are specific to the items in a layout area.

Slider Attributes

Attributes that are specific to sliders.

