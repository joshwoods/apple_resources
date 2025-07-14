

- BrowserEngineKit
- BEAccessibility
-  valueChangedNotification 

Type Property

# valueChangedNotification

The notification you post when the value of an element changes.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
static var valueChangedNotification: UIAccessibility.Notification
```

## Overview

Post this notification when the value of an input element changes, when someone or a script adds text to a text control or removes text from a text control, or when the `aria-valuenow` or `aria-valuetext` attributes of an element change.

If an element contains a text selection and the content changes, or the editing cursor position changes, post this notification followed by selectionChangedNotification for the element.

## See Also

### Accessibility

protocol BEAccessibilityTextMarkerSupport

A set of methods that provide information about text offsets to support assistive features.

static var selectionChangedNotification: UIAccessibility.Notification

The notification you post when the selection inside an element changes.

struct BEAccessibilityContainerType

An enumeration that indicates the type of container in which an element is located.

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

