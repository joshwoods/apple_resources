

- XCUIAutomation
-  XCUIElementSnapshot 

Protocol

# XCUIElementSnapshot

A set of attributes to express a snapshot of an element’s attributes and descendant user interface hierarchy.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
protocol XCUIElementSnapshot : XCUIElementAttributes
```

## Topics

### Inspecting attributes

var children: [any XCUIElementSnapshot]

An array of descendant user interface element snapshots.

**Required**

var dictionaryRepresentation: [XCUIElement.AttributeName : Any]

A hierarchical dictionary representation of an element’s attributes, and all of an element’s user interface descendants.

**Required**

## Relationships

### Inherits From

- XCUIElementAttributes

## See Also

### UI elements

class XCUIElement

A UI element in an application.

protocol XCUIElementAttributes

Attributes exposed by UI elements.

protocol XCUIElementSnapshotProviding

A method to capture a snapshot of an element’s attributes and descendant user interface hierarchy.

class XCUICoordinate

A location on screen relative to a UI element.

