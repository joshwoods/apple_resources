

- AppKit
- NSAccessibility
-  NSAccessibility.Attribute 

Structure

# NSAccessibility.Attribute

Constants that describe attributes.

macOS

``` source
struct Attribute
```

## Topics

### Attributes

static let activationPoint: NSAccessibility.Attribute

static let allowedValues: NSAccessibility.Attribute

The allowed values in the slider (`NSArray`).

Deprecated

static let alternateUIVisible: NSAccessibility.Attribute

static let cancelButton: NSAccessibility.Attribute

The element that represents the cancel button (`id`).

static let children: NSAccessibility.Attribute

The element’s child elements in the accessibility hierarchy (`NSArray`).

Deprecated

static let clearButton: NSAccessibility.Attribute

The element that represents the clear button in a search field (`id`).

Deprecated

static let closeButton: NSAccessibility.Attribute

The element representing the close button (`id`).

Deprecated

static let columnCount: NSAccessibility.Attribute

The number of columns in the grid (`NSNumber` as `intValue`).

Deprecated

static let columnHeaderUIElements: NSAccessibility.Attribute

The table’s column headers (`NSArray`).

static let columnIndexRange: NSAccessibility.Attribute

The column index range of the cell (an `NSValue` instance that contains the row’s starting index and index span in the table).

static let columnTitles: NSAccessibility.Attribute

The elements that represent the column titles (`NSArray`).

static let columns: NSAccessibility.Attribute

The table’s columns (`NSArray`).

static let containsProtectedContent: NSAccessibility.Attribute

A flag that indicates whether the object contains protected content (true), or not (false) (`NSNumber` as `boolValue`).

static let contents: NSAccessibility.Attribute

Elements that represent the contents in the current element, such as the document view of a scroll view (`NSArray`).

static let criticalValue: NSAccessibility.Attribute

The critical value in a level indicator (typically, `NSNumber`).

static let decrementButton: NSAccessibility.Attribute

The element that represents a stepper’s decrement button (`id`).

static let defaultButton: NSAccessibility.Attribute

The element that represents the default button (`id`).

static let description: NSAccessibility.Attribute

The purpose of the element, not including the role (`NSString`).

static let disclosedByRow: NSAccessibility.Attribute

The row disclosing this row (`id`).

Deprecated

static let disclosedRows: NSAccessibility.Attribute

The rows disclosed by this row (`NSArray`).

static let disclosing: NSAccessibility.Attribute

A flag that indicates whether a row is disclosing other rows (`NSNumber`).

static let disclosureLevel: NSAccessibility.Attribute

The indentation level of this row (`NSNumber`).

static let document: NSAccessibility.Attribute

The URL for the file represented by the element (`NSString`).

static let edited: NSAccessibility.Attribute

A flag that indicates whether the element has been modified (`NSNumber`).

static let enabled: NSAccessibility.Attribute

A flag that indicates the enabled state of the element (`NSNumber`).

static let expanded: NSAccessibility.Attribute

A flag that indicates whether the element is expanded (`NSNumber`).

static let extrasMenuBar: NSAccessibility.Attribute

The app extras menu bar (`id`).

static let filename: NSAccessibility.Attribute

The filename associated with the element (`NSString`).

static let focused: NSAccessibility.Attribute

A flag that indicates the presence of keyboard focus (`NSNumber`).

static let focusedUIElement: NSAccessibility.Attribute

The element with the current focus (`id`).

Deprecated

static let focusedWindow: NSAccessibility.Attribute

The app’s window that has current focus (`id`).

static let frontmost: NSAccessibility.Attribute

A flag that indicates whether the app is frontmost (`NSNumber`).

static let fullScreenButton: NSAccessibility.Attribute

The element that represents the full-screen button (`id`).

static let growArea: NSAccessibility.Attribute

The element representing the grow area (`id`).

static let handles: NSAccessibility.Attribute

The drag handles of the item (`NSArray`).

Deprecated

static let header: NSAccessibility.Attribute

The element that represents a table view’s header (`id`).

static let help: NSAccessibility.Attribute

The help text for the element (`NSString`).

static let hidden: NSAccessibility.Attribute

A flag that indicates whether the app is hidden (`NSNumber`).

static let horizontalScrollBar: NSAccessibility.Attribute

The element that represents a scroll view’s horizontal scroll bar (`id`).

static let horizontalUnitDescription: NSAccessibility.Attribute

The description of the layout view’s horizontal units (`NSString`).

static let horizontalUnits: NSAccessibility.Attribute

The units that the layout view uses for horizontal values (`NSString`). See Measurement unit attributes for possible values.

Deprecated

static let identifier: NSAccessibility.Attribute

The identity of the element (`NSString`).

static let incrementButton: NSAccessibility.Attribute

The element that represents a stepper’s increment button (`id`).

static let index: NSAccessibility.Attribute

The index of the row or column represented by the element (`NSValue`).

static let insertionPointLineNumber: NSAccessibility.Attribute

The line number containing the insertion point (`NSNumber`).

Deprecated

static let labelUIElements: NSAccessibility.Attribute

The elements that represent the slider’s labels (`NSArray`).

static let labelValue: NSAccessibility.Attribute

The value of the label represented by this element (`NSNumber`).

static let linkedUIElements: NSAccessibility.Attribute

The elements with which this element is related (`NSArray`).

Deprecated

static let main: NSAccessibility.Attribute

A flag that indicates whether the window is the main window (`NSNumber`).

static let mainWindow: NSAccessibility.Attribute

The app’s main window (`id`).

static let markerGroupUIElement: NSAccessibility.Attribute

A marker group user interface element (`id`).

Deprecated

static let markerType: NSAccessibility.Attribute

The type of the marker (`NSString`). See Ruler Marker Type Values for possible values.

static let markerTypeDescription: NSAccessibility.Attribute

The description of the marker type (`NSString`).

static let markerUIElements: NSAccessibility.Attribute

An array of marker user interface elements (`NSArray`)

static let markerValues: NSAccessibility.Attribute

The marker values (`NSArray` of `NSNumber`).

static let matteContentUIElement: NSAccessibility.Attribute

The element that is clipped by the matte (`id`).

Deprecated

static let matteHole: NSAccessibility.Attribute

The bounds of the matte hole, in screen coordinates in points (`NSValue` containing an `NSRect`).

Deprecated

static let maxValue: NSAccessibility.Attribute

The element’s maximum value (`id`).

static let menuBar: NSAccessibility.Attribute

The app’s menu bar (`id`).

static let minValue: NSAccessibility.Attribute

The element’s minimum value (`id`).

static let minimizeButton: NSAccessibility.Attribute

The element that represents the minimize button (`id`).

static let minimized: NSAccessibility.Attribute

A flag that indicates whether the window is minimized (`NSNumber`).

static let modal: NSAccessibility.Attribute

A flag that indicates whether the window represented by this element is modal (`NSNumber`).

static let nextContents: NSAccessibility.Attribute

The elements representing the contents that follow the current divider element, such as a subview adjacent to a split view’s splitter element (`NSArray`).

static let numberOfCharacters: NSAccessibility.Attribute

The number of characters in the text (`NSNumber`).

static let orderedByRow: NSAccessibility.Attribute

A flag that indicates whether the grid is ordered row major (true), or column major (false) (`NSNumber` as `boolValue`).

static let orientation: NSAccessibility.Attribute

The element’s orientation, which can have the value horizontal or vertical.

static let overflowButton: NSAccessibility.Attribute

The element that represents a toolbar’s overflow button (`id`).

static let parent: NSAccessibility.Attribute

The element’s parent element in the accessibility hierarchy (`id`).

static let placeholderValue: NSAccessibility.Attribute

The placeholder value for a control, such as a text field (`NSString`).

static let position: NSAccessibility.Attribute

The position in points of the element’s lower-left corner in screen-relative coordinates (`NSValue`).

static let previousContents: NSAccessibility.Attribute

The elements representing the contents that precede the current divider element, such as a subview adjacent to a split view’s splitter bar element (`NSArray`).

static let proxy: NSAccessibility.Attribute

The element that represents the window’s proxy icon (`id`).

static let required: NSAccessibility.Attribute

static let role: NSAccessibility.Attribute

The element’s type, such as `NSAccessibilityRadioButtonRole` (`NSString`). See Roles for a list of available roles.

static let roleDescription: NSAccessibility.Attribute

A localized, human-intelligible description of the element’s role, such as `radio button` (`NSString`).

static let rowCount: NSAccessibility.Attribute

The number of rows in the grid (`NSNumber` as `intValue`).

static let rowHeaderUIElements: NSAccessibility.Attribute

The table’s row headers (`NSArray`).

static let rowIndexRange: NSAccessibility.Attribute

The row index range of the cell (an `NSValue` instance that contains the row’s starting index and index span in the table).

Deprecated

static let rows: NSAccessibility.Attribute

The table’s rows (`NSArray`).

static let searchButton: NSAccessibility.Attribute

The element that represents the search button in a search field (`id`).

static let searchMenu: NSAccessibility.Attribute

The element that represents the menu in a search field (`id`).

static let selected: NSAccessibility.Attribute

A flag that indicates whether the element is selected (`NSNumber`).

static let selectedCells: NSAccessibility.Attribute

The table’s selected cells (`NSArray`). This attribute is required for cell-based tables.

Deprecated

static let selectedChildren: NSAccessibility.Attribute

The currently selected children of the element (`NSArray`).

static let selectedColumns: NSAccessibility.Attribute

The table’s selected columns (`NSArray`).

static let selectedRows: NSAccessibility.Attribute

The table’s selected rows (`NSArray`).

static let selectedText: NSAccessibility.Attribute

The currently selected text (`NSString`).

static let selectedTextRange: NSAccessibility.Attribute

The range of selected text (`NSValue`).

static let selectedTextRanges: NSAccessibility.Attribute

An array of `NSValue` (`rangeValue`) ranges of selected text (`NSArray`).

static let servesAsTitleForUIElements: NSAccessibility.Attribute

The elements for which this element serves as the title (`NSArray`).

static let sharedCharacterRange: NSAccessibility.Attribute

The (`rangeValue`) part of shared text in this view (`NSValue`).

static let sharedFocusElements: NSAccessibility.Attribute

static let sharedTextUIElements: NSAccessibility.Attribute

The elements with which the text of this element is shared (`NSArray`).

static let shownMenu: NSAccessibility.Attribute

The menu currently being displayed (`id`).

static let size: NSAccessibility.Attribute

The element’s size in points (`NSValue`).

static let sortDirection: NSAccessibility.Attribute

The column’s sort direction (`NSString`). See Column Sort Direction for possible values.

static let splitters: NSAccessibility.Attribute

The views and splitter bar in a split view (`NSArray`).

static let subrole: NSAccessibility.Attribute

The element’s subrole, such as `NSAccessibilityTableRowSubrole` (`NSString`). See Subroles for a list of available subroles.

static let tabs: NSAccessibility.Attribute

The tab elements in a tab view (`NSArray`).

static let title: NSAccessibility.Attribute

The title of the element, such as a button’s visible text (`NSString`).

static let titleUIElement: NSAccessibility.Attribute

An element that represents another element’s static text title (`id`).

static let toolbarButton: NSAccessibility.Attribute

The element that represents the toolbar button (`id`).

static let topLevelUIElement: NSAccessibility.Attribute

The top-level element that contains this element (`id`).

static let unitDescription: NSAccessibility.Attribute

The description of ruler units (`NSString`).

static let units: NSAccessibility.Attribute

The ruler units (`NSString`). See Measurement Unit Attributes for possible values.

static let url: NSAccessibility.Attribute

The URL associated with the element (`NSURL`).

static let value: NSAccessibility.Attribute

The element’s value (`id`).

static let valueDescription: NSAccessibility.Attribute

The description of the element’s value (`NSString`).

static let verticalScrollBar: NSAccessibility.Attribute

The element that represents the vertical scroll bar in a scroll view (`id`).

static let verticalUnitDescription: NSAccessibility.Attribute

The description of the layout view’s vertical units (`NSString`).

static let verticalUnits: NSAccessibility.Attribute

The units that the layout view uses for vertical values (`NSString`). See Measurement unit attributes for possible values.

static let visibleCells: NSAccessibility.Attribute

The table’s visible cells (`NSArray`). This attribute is required for cell-based tables.

static let visibleCharacterRange: NSAccessibility.Attribute

The range of visible text (`NSValue`).

static let visibleChildren: NSAccessibility.Attribute

The element’s child elements that are visible (`NSArray`).

static let visibleColumns: NSAccessibility.Attribute

The table’s visible columns (`NSArray`).

static let visibleRows: NSAccessibility.Attribute

The table’s visible rows (`NSArray`).

static let warningValue: NSAccessibility.Attribute

The warning value in a level indicator (typically, `NSNumber`).

static let window: NSAccessibility.Attribute

The window containing the current element (`id`).

static let windows: NSAccessibility.Attribute

The app’s windows (`NSArray`).

static let zoomButton: NSAccessibility.Attribute

The element that represents the zoom button (`id`).

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessibility Types

struct Action

Constants that describe types of actions.

struct AnnotationAttributeKey

Keys for annotation attributes.

enum NSAccessibilityAnnotationPosition

Constants that specify the position where the annotation applies.

struct FontAttributeKey

Keys for font attributes.

enum NSAccessibilityOrientation

Values that indicate the orientation of accessibility elements, such as scroll bars and split views.

struct OrientationValue

Values that indicate the orientation of user interface elements, such as scroll bars and split views.

struct ParameterizedAttribute

Values that describe parameterized attributes.

struct Role

Values that describe types of objects that accessibility elements represent.

enum NSAccessibilityRulerMarkerType

Values that indicate the marker type of an accessibility element.

struct RulerMarkerTypeValue

Values that describe ruler marker types.

struct RulerUnitValue

Values that indicate the unit values of a ruler or layout area.

struct SortDirectionValue

Values that indicate the sort direction of a column.

enum NSAccessibilitySortDirection

Values that indicate the sort direction of a column.

struct Subrole

Values that describe specialized object subtypes that accessibility elements represent.

enum NSAccessibilityUnits

Values that indicate the unit values of a ruler or layout area.

