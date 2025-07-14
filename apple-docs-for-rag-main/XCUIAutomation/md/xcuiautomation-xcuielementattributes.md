

- XCUIAutomation
-  XCUIElementAttributes 

Protocol

# XCUIElementAttributes

Attributes exposed by UI elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
protocol XCUIElementAttributes
```

## Overview

The XCUIElementAttributes protocol adds attribute-related functionality to the XCUIElement class. Access these properties on an instance of XCUIElement to query the current state of the UI element’s attributes.

Note

The attributes provided by this protocol represent data exposed to the Accessibility system, and are available during query matching.

## Topics

### Identity

var identifier: String

The element’s accessibility identifier.

**Required**

var elementType: XCUIElement.ElementType

The type of the element.

**Required**

enum ElementType

The types of UI elements that you find, inspect, and interact with in a UI test.

### Value

var value: Any?

The raw value attribute of the element.

**Required**

var placeholderValue: String?

The value displayed when the element has no value.

**Required**

var title: String

The title attribute of the element.

**Required**

var label: String

The label attribute of the element.

**Required**

### Interaction state

var hasFocus: Bool

The property that determines whether the element has UI focus.

**Required**

var isEnabled: Bool

Whether or not the element is enabled for user interaction.

**Required**

var isSelected: Bool

The property that determines whether the element is selected.

**Required**

### Size

var frame: CGRect

The frame of the element in the screen’s coordinate space.

**Required**

var horizontalSizeClass: XCUIElement.SizeClass

The horizontal size class of the element.

**Required**

var verticalSizeClass: XCUIElement.SizeClass

The vertical size class of the element.

**Required**

enum SizeClass

The user interface size classes you can inspect in a UI test.

## Relationships

### Inherited By

- XCUIElementSnapshot

### Conforming Types

- XCUIApplication
- XCUIElement

## See Also

### UI elements

class XCUIElement

A UI element in an application.

protocol XCUIElementSnapshot

A set of attributes to express a snapshot of an element’s attributes and descendant user interface hierarchy.

protocol XCUIElementSnapshotProviding

A method to capture a snapshot of an element’s attributes and descendant user interface hierarchy.

class XCUICoordinate

A location on screen relative to a UI element.

