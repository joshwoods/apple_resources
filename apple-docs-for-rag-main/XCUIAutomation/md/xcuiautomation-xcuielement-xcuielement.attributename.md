

- XCUIAutomation
- XCUIElement
-  XCUIElement.AttributeName 

Structure

# XCUIElement.AttributeName

A set of string constants that serve as keys for storing element attributes in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
struct AttributeName
```

## Topics

### Keys

static let children: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s children.

static let elementType: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s type.

static let enabled: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying whether an element is enabled.

static let frame: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s frame.

static let hasFocus: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying whether an element has focus.

static let horizontalSizeClass: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s horizontal size class.

static let identifier: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s identifier.

static let label: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s label.

static let placeholderValue: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s placeholder value.

static let selected: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying whether an element is selected.

static let title: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s title.

static let value: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s value.

static let verticalSizeClass: XCUIElement.AttributeName

A string constant that serves as a dictionary key identifying an element’s vertical size class.

### Initializers

init(rawValue: String)

Creates an attribute name dictionary key from a string value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting types

enum ElementType

The types of UI elements that you find, inspect, and interact with in a UI test.

enum SizeClass

The user interface size classes you can inspect in a UI test.

