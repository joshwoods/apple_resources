

- AppKit
- NSAccessibility
-  NSAccessibility.Action 

Structure

# NSAccessibility.Action

Constants that describe types of actions.

macOS

``` source
struct Action
```

## Topics

### Actions

static let cancel: NSAccessibility.Action

An action that cancels the operation.

static let confirm: NSAccessibility.Action

An action that simulates pressing Return in the object, such as a text field.

Deprecated

static let decrement: NSAccessibility.Action

An action that decrements the value of the object.

static let delete: NSAccessibility.Action

An action that deletes the value of the object.

static let increment: NSAccessibility.Action

An action that increments the value of the object.

static let pick: NSAccessibility.Action

An action that selects the object, such as a menu item.

static let press: NSAccessibility.Action

An action that simulates clicking an object, such as a button.

static let raise: NSAccessibility.Action

An action that simulates bringing a window forward by clicking on its title bar.

static let showAlternateUI: NSAccessibility.Action

An action that shows an alternate UI, for example, during a mouse-hover event.

static let showDefaultUI: NSAccessibility.Action

An action that shows the original or default UI; for example, during a mouse-hover event.

static let showMenu: NSAccessibility.Action

An action that simulates showing a menu by clicking on it.

### Descriptions

var description: String?

Returns a standard description for an action.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessibility Types

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

