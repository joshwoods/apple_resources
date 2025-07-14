

- AppKit
- NSAccessibility
-  NSAccessibility.Role 

Structure

# NSAccessibility.Role

Values that describe types of objects that accessibility elements represent.

macOS

``` source
struct Role
```

## Topics

### Roles

static let application: NSAccessibility.Role

The app role.

static let browser: NSAccessibility.Role

The browser role.

static let busyIndicator: NSAccessibility.Role

The busy indicator role.

static let button: NSAccessibility.Role

The button role.

static let cell: NSAccessibility.Role

The cell role in a table or matrix.

static let checkBox: NSAccessibility.Role

The checkbox role.

static let colorWell: NSAccessibility.Role

The color well role.

static let column: NSAccessibility.Role

The column role.

static let comboBox: NSAccessibility.Role

The combo box role.

static let disclosureTriangle: NSAccessibility.Role

The disclosure triangle role.

static let drawer: NSAccessibility.Role

The drawer role.

static let grid: NSAccessibility.Role

The grid role.

static let group: NSAccessibility.Role

The group role.

static let growArea: NSAccessibility.Role

The grow (resize) area role in a window.

static let handle: NSAccessibility.Role

The drag handle role.

static let helpTag: NSAccessibility.Role

The help tag role.

static let image: NSAccessibility.Role

The image role.

static let incrementor: NSAccessibility.Role

The stepper role.

static let layoutArea: NSAccessibility.Role

The layout area role (a view, such as a graphic view, that contains visual elements that may not have any accessibility representation).

static let layoutItem: NSAccessibility.Role

The role for an item in a layout area.

static let levelIndicator: NSAccessibility.Role

The level indicator role.

static let link: NSAccessibility.Role

The link role.

static let list: NSAccessibility.Role

The list role.

static let matte: NSAccessibility.Role

The matte role.

static let menu: NSAccessibility.Role

The menu role.

static let menuBar: NSAccessibility.Role

The menu bar role.

static let menuBarItem: NSAccessibility.Role

The menu bar item role.

static let menuButton: NSAccessibility.Role

The menu button role.

static let menuItem: NSAccessibility.Role

The menu item role.

static let outline: NSAccessibility.Role

The outline role.

static let pageRole: NSAccessibility.Role

The page role.

static let popUpButton: NSAccessibility.Role

The pop-up button role.

static let popover: NSAccessibility.Role

The popover role.

static let progressIndicator: NSAccessibility.Role

The progress indicator role.

static let radioButton: NSAccessibility.Role

The radio button role.

static let radioGroup: NSAccessibility.Role

The radio button group role.

static let relevanceIndicator: NSAccessibility.Role

The relevance indicator role.

static let row: NSAccessibility.Role

The row role.

static let ruler: NSAccessibility.Role

The ruler role.

static let rulerMarker: NSAccessibility.Role

The ruler marker role.

static let scrollArea: NSAccessibility.Role

The scroll view role.

static let scrollBar: NSAccessibility.Role

The scroll bar role.

static let sheet: NSAccessibility.Role

The sheet role.

static let slider: NSAccessibility.Role

The slider role.

static let splitGroup: NSAccessibility.Role

The split view role.

static let splitter: NSAccessibility.Role

The splitter bar role for a split view.

static let staticText: NSAccessibility.Role

The uneditable text role.

static let systemWide: NSAccessibility.Role

The systemwide accessibility object role.

static let tabGroup: NSAccessibility.Role

The tab group role.

static let table: NSAccessibility.Role

The table role.

static let textArea: NSAccessibility.Role

The text view role.

static let textField: NSAccessibility.Role

The text field role.

static let toolbar: NSAccessibility.Role

The toolbar role.

static let valueIndicator: NSAccessibility.Role

The value indicator role.

static let window: NSAccessibility.Role

The window role.

static let unknown: NSAccessibility.Role

An object with an unknown role.

### Descriptions

func description(with: NSAccessibility.Subrole?) -> String?

Returns a standard description for a role and subrole.

static func description(for: Any) -> String?

Returns a standard role description for a user interface element.

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

struct Attribute

Constants that describe attributes.

struct FontAttributeKey

Keys for font attributes.

enum NSAccessibilityOrientation

Values that indicate the orientation of accessibility elements, such as scroll bars and split views.

struct OrientationValue

Values that indicate the orientation of user interface elements, such as scroll bars and split views.

struct ParameterizedAttribute

Values that describe parameterized attributes.

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

