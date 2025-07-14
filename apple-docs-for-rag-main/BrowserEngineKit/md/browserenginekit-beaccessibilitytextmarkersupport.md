

- BrowserEngineKit
-  BEAccessibilityTextMarkerSupport 

Protocol

# BEAccessibilityTextMarkerSupport

A set of methods that provide information about text offsets to support assistive features.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
protocol BEAccessibilityTextMarkerSupport : NSObjectProtocol
```

## Overview

In your alternative browser engine, implement `BEAccessibilityTextMarkerSupport` on views that represent elements in the Document Object Model (DOM) to supply accessibility information about the element’s text to the system.

## Topics

### Text positions

func accessibilityNextTextMarker(BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that follows the given text marker.

**Required**

func accessibilityPreviousTextMarker(BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that precedes the given text marker.

**Required**

func accessibilityLineStartMarker(for: BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that represents the start of the line that contains the given text marker.

**Required**

func accessibilityLineEndMarker(for: BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that represents the end of the line that contains the given text marker.

**Required**

func accessibilityMarker(for: CGPoint) -> BEAccessibilityTextMarker?

Returns the text marker at a point in the view’s coordinate system.

**Required**

func accessibilityTextMarker(forPosition: Int) -> BEAccessibilityTextMarker?

Returns the text marker for the text at a given index in the element’s text.

**Required**

class BEAccessibilityTextMarker

An abstract class that represents a location in an element’s accessibility text.

### Text ranges

func accessibilityBounds(for: BEAccessibilityTextMarker.Range) -> CGRect

Calculates the bounding rectangle for a text range.

**Required**

func accessibilityTextMarkerRange() -> BEAccessibilityTextMarker.Range

The text marker range of the current element.

**Required**

func accessibilityTextMarkerRangeForCurrentSelection() -> BEAccessibilityTextMarker.Range?

The text marker range of the current selection.

**Required**

func accessibilityTextMarkerRange(for: NSRange) -> BEAccessibilityTextMarker.Range?

Returns the text marker range for the text in a given range.

**Required**

func accessibilityRange(for: BEAccessibilityTextMarker.Range) -> NSRange

Returns the range for the text in a given accessibility marker range.

**Required**

class Range

A class that represents a range in an element’s accessibility text.

### Instance Methods

func accessibilityContent(for: BEAccessibilityTextMarker.Range) -> String?

Returns the accessibility content for a text range.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Accessibility

static var valueChangedNotification: UIAccessibility.Notification

The notification you post when the value of an element changes.

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

