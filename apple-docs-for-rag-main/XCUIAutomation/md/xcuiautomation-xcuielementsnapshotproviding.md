

- XCUIAutomation
-  XCUIElementSnapshotProviding 

Protocol

# XCUIElementSnapshotProviding

A method to capture a snapshot of an element’s attributes and descendant user interface hierarchy.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
protocol XCUIElementSnapshotProviding : NSObjectProtocol
```

## Topics

### Providing snapshots

func snapshot() throws -> any XCUIElementSnapshot

Returns a snapshot of an element’s attributes and descendant user interface hierarchy.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- XCUIApplication
- XCUIElement

## See Also

### UI elements

class XCUIElement

A UI element in an application.

protocol XCUIElementAttributes

Attributes exposed by UI elements.

protocol XCUIElementSnapshot

A set of attributes to express a snapshot of an element’s attributes and descendant user interface hierarchy.

class XCUICoordinate

A location on screen relative to a UI element.

