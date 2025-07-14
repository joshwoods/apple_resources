

- BrowserEngineKit
-  BEAccessibilityPressedState 

Enumeration

# BEAccessibilityPressedState

An enumeration that indicates whether an element is pressed.

iOS 18.0+iPadOS 18.0+macOStvOS 18.0+visionOS 2.0+

``` source
enum BEAccessibilityPressedState
```

## Topics

### Element states

case `false`

The element isn’t pressed.

case `true`

The element is pressed.

case mixed

The element is in a mixed state.

case undefined

The element is in an undefined state.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessibility

protocol BEAccessibilityTextMarkerSupport

A set of methods that provide information about text offsets to support assistive features.

static var valueChangedNotification: UIAccessibility.Notification

The notification you post when the value of an element changes.

static var selectionChangedNotification: UIAccessibility.Notification

The notification you post when the selection inside an element changes.

struct BEAccessibilityContainerType

An enumeration that indicates the type of container in which an element is located.

static var menuItem: UIAccessibilityTraits

The accessibility element behaves like a menu item.

static var popUpButton: UIAccessibilityTraits

The accessibility element behaves like a pop-up button.

static var radioButton: UIAccessibilityTraits

The accessibility element behaves like a radio button.

static var readOnly: UIAccessibilityTraits

The accessibility element is read-only.

static var visited: UIAccessibilityTraits

The accessibility element behaves like a link that someone previously visited.

