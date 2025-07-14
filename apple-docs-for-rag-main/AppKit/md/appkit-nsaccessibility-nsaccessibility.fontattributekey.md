

- AppKit
- NSAccessibility
-  NSAccessibility.FontAttributeKey 

Structure

# NSAccessibility.FontAttributeKey

Keys for font attributes.

macOS

``` source
struct FontAttributeKey
```

## Topics

### Font Attributes

static let fontFamily: NSAccessibility.FontAttributeKey

An optional key for a font family.

static let fontName: NSAccessibility.FontAttributeKey

A required key for a font name.

static let fontSize: NSAccessibility.FontAttributeKey

A required key for a font size.

static let visibleName: NSAccessibility.FontAttributeKey

An optional key for font visibility.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

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

