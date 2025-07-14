

- AppKit
- Deprecated Symbols
- NSAccessibility
-  Standard Attributes 

API Collection

# Standard Attributes

Standard attributes that can be adopted by any accessibility object.

## Topics

### Constants

static let children: NSAccessibility.Attribute

The element’s child elements in the accessibility hierarchy (`NSArray`).

Deprecated

static let contents: NSAccessibility.Attribute

Elements that represent the contents in the current element, such as the document view of a scroll view (`NSArray`).

static let description: NSAccessibility.Attribute

The purpose of the element, not including the role (`NSString`).

static let enabled: NSAccessibility.Attribute

A flag that indicates the enabled state of the element (`NSNumber`).

static let focused: NSAccessibility.Attribute

A flag that indicates the presence of keyboard focus (`NSNumber`).

static let help: NSAccessibility.Attribute

The help text for the element (`NSString`).

static let maxValue: NSAccessibility.Attribute

The element’s maximum value (`id`).

static let minValue: NSAccessibility.Attribute

The element’s minimum value (`id`).

static let parent: NSAccessibility.Attribute

The element’s parent element in the accessibility hierarchy (`id`).

static let position: NSAccessibility.Attribute

The position in points of the element’s lower-left corner in screen-relative coordinates (`NSValue`).

static let role: NSAccessibility.Attribute

The element’s type, such as `NSAccessibilityRadioButtonRole` (`NSString`). See Roles for a list of available roles.

static let roleDescription: NSAccessibility.Attribute

A localized, human-intelligible description of the element’s role, such as `radio button` (`NSString`).

static let selectedChildren: NSAccessibility.Attribute

The currently selected children of the element (`NSArray`).

static let shownMenu: NSAccessibility.Attribute

The menu currently being displayed (`id`).

static let size: NSAccessibility.Attribute

The element’s size in points (`NSValue`).

static let subrole: NSAccessibility.Attribute

The element’s subrole, such as `NSAccessibilityTableRowSubrole` (`NSString`). See Subroles for a list of available subroles.

static let title: NSAccessibility.Attribute

The title of the element, such as a button’s visible text (`NSString`).

static let topLevelUIElement: NSAccessibility.Attribute

The top-level element that contains this element (`id`).

static let value: NSAccessibility.Attribute

The element’s value (`id`).

static let valueDescription: NSAccessibility.Attribute

The description of the element’s value (`NSString`).

static let visibleChildren: NSAccessibility.Attribute

The element’s child elements that are visible (`NSArray`).

static let window: NSAccessibility.Attribute

The window containing the current element (`id`).

## See Also

### Constants

Text-Specific Attributes

Attributes that are specific to text.

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

