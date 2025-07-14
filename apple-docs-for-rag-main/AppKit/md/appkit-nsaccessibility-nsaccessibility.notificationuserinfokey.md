

- AppKit
- NSAccessibility
-  NSAccessibility.NotificationUserInfoKey 

Structure

# NSAccessibility.NotificationUserInfoKey

The key in the user info dictionary for a notification.

macOS

``` source
struct NotificationUserInfoKey
```

## Topics

### Constants

static let announcement: NSAccessibility.NotificationUserInfoKey

The announcement as a localized string.

static let uiElements: NSAccessibility.NotificationUserInfoKey

An array of elements for the notification.

static let priority: NSAccessibility.NotificationUserInfoKey

A priority level that can help an assistive app determine how to handle the corresponding notification.

enum NSAccessibilityPriorityLevel

A data type for notification priority levels.

### Initializers

init(rawValue: String)

Returns a new notification object with a specified name and object.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Using Accessibility Types

struct Action

Constants that describe types of actions.

struct AnnotationAttributeKey

Keys for annotation attributes.

struct Attribute

Constants that describe attributes.

struct FontAttributeKey

Keys for font attributes.

struct Notification

The name of the notification.

struct OrientationValue

Values that indicate the orientation of user interface elements, such as scroll bars and split views.

struct ParameterizedAttribute

Values that describe parameterized attributes.

struct Role

Values that describe types of objects that accessibility elements represent.

struct RulerMarkerTypeValue

Values that describe ruler marker types.

struct RulerUnitValue

Values that indicate the unit values of a ruler or layout area.

struct SortDirectionValue

Values that indicate the sort direction of a column.

struct Subrole

Values that describe specialized object subtypes that accessibility elements represent.

