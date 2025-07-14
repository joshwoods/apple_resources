

- BrowserEngineKit
-  BEAccessibilityContainerType 

Structure

# BEAccessibilityContainerType

An enumeration that indicates the type of container in which an element is located.

iOS 18.0+iPadOS 18.0+macOStvOS 18.0+visionOS 2.0+

``` source
struct BEAccessibilityContainerType
```

## Overview

Set a value from this enumeration for an element’s browserAccessibilityContainerType property to indicate the type of container in which the element is located. For example, set table as the `browserAccessibilityContainerType` for an element within a table cell.

## Topics

### Container types

static var landmark: BEAccessibilityContainerType

A website accessibility landmark contains the element.

static var table: BEAccessibilityContainerType

A table contains the element.

static var list: BEAccessibilityContainerType

A list contains the element.

static var fieldset: BEAccessibilityContainerType

An HTML fieldset element contains the element.

static var dialog: BEAccessibilityContainerType

A dialog contains the element.

static var tree: BEAccessibilityContainerType

A tree contains the element.

static var frame: BEAccessibilityContainerType

A frame contains the element.

static var article: BEAccessibilityContainerType

An HTML article element contains the alert.

static var semanticGroup: BEAccessibilityContainerType

A semantic group contains the element.

static var scrollArea: BEAccessibilityContainerType

A scroll area contains the element.

static var alert: BEAccessibilityContainerType

An alert contains the element.

static var descriptionList: BEAccessibilityContainerType

A description list contains the element.

### Initializers

init(rawValue: UInt)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessibility

protocol BEAccessibilityTextMarkerSupport

A set of methods that provide information about text offsets to support assistive features.

static var valueChangedNotification: UIAccessibility.Notification

The notification you post when the value of an element changes.

static var selectionChangedNotification: UIAccessibility.Notification

The notification you post when the selection inside an element changes.

enum BEAccessibilityPressedState

An enumeration that indicates whether an element is pressed.

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

