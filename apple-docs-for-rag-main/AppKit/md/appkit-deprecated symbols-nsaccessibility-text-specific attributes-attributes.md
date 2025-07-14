

- AppKit
- Deprecated Symbols
- NSAccessibility
-  Text-Specific Attributes 

API Collection

# Text-Specific Attributes

Attributes that are specific to text.

## Topics

### Constants

static let insertionPointLineNumber: NSAccessibility.Attribute

The line number containing the insertion point (`NSNumber`).

Deprecated

static let numberOfCharacters: NSAccessibility.Attribute

The number of characters in the text (`NSNumber`).

static let selectedText: NSAccessibility.Attribute

The currently selected text (`NSString`).

static let selectedTextRange: NSAccessibility.Attribute

The range of selected text (`NSValue`).

static let selectedTextRanges: NSAccessibility.Attribute

An array of `NSValue` (`rangeValue`) ranges of selected text (`NSArray`).

static let sharedCharacterRange: NSAccessibility.Attribute

The (`rangeValue`) part of shared text in this view (`NSValue`).

static let sharedTextUIElements: NSAccessibility.Attribute

The elements with which the text of this element is shared (`NSArray`).

static let visibleCharacterRange: NSAccessibility.Attribute

The range of visible text (`NSValue`).

## See Also

### Constants

Standard Attributes

Standard attributes that can be adopted by any accessibility object.

Text-Specific Parameterized Attributes

Parameterized attributes specific to text.

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

