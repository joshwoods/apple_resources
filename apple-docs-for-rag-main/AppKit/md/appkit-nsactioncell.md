

- AppKit
-  NSActionCell 

Class

# NSActionCell

An active area inside a control.

macOS

``` source
@MainActor
class NSActionCell
```

## Overview

An NSActionCell does three things: it displays text or an icon; it provides the target object and action method used by its NSControl object; and it handles mouse (cursor) tracking by properly highlighting its area and sending action messages to its target based on cursor movement.

The controlView of an NSActionCell is the view in which the receiver was last drawn.

### Obtaining and Setting Cell Values

The floatValue, intValue, and integerValue methods return the value with their corresponding types after validating any editing of cell content. If the cell is not a text-type cell or the cell value is not scannable to the appropriate type, these return 0.

The stringValue method returns the receiver’s value as a string object as converted by the cell’s formatter, if one exists. If no formatter exists and the value is an NSString, returns the value as a plain, attributed, or localized formatted string. If the value is not an `NSString` or cannot be converted to one, returns an empty string. The method supplements the NSCell implementation by validating and retaining any editing changes being made to cell text.

Calling `setObjectValue:` discards any editing of the receiver’s text and sets its object value to the specified object. After doing so, if the object value is different from what it was before the method was invoked, the method marks the receiver as needing redisplay.

### Configuring an NSActionCell Object

The `NSActionCell` implementation of setFloatingPointFormat:left:right: supplements the `NSCell` implementation by marking the receiver as needing redisplay after discarding any editing changes that were being made to cell text.

## Topics

### Assigning the Target and Action

var action: Selector?

Returns the receiver’s action-message selector.

var target: AnyObject?

Returns the receiver’s target object.

### Assigning a Tag

var tag: Int

Returns the receiver’s tag.

## Relationships

### Inherits From

- NSCell

### Inherited By

- NSButtonCell
- NSDatePickerCell
- NSFormCell
- NSLevelIndicatorCell
- NSPathCell
- NSSegmentedCell
- NSSliderCell
- NSStepperCell
- NSTextFieldCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification

## See Also

### View Fundamentals

class NSView

The infrastructure for drawing, printing, and handling events in an app.

class NSControl

A specialized view, such as a button or text field, that notifies your app of relevant events using the target-action design pattern.

class NSCell

A mechanism for displaying text or images in a view object without the overhead of a full NSView subclass.

