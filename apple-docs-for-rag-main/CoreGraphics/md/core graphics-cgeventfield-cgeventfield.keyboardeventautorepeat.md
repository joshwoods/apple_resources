

- Core Graphics
- CGEventField
-  CGEventField.keyboardEventAutorepeat 

Case

# CGEventField.keyboardEventAutorepeat

Key to access an integer field, non-zero when this is an autorepeat of a key-down, and zero otherwise.

Mac CatalystmacOS

``` source
case keyboardEventAutorepeat
```

## See Also

### Constants

case mouseEventNumber

Key to access an integer field that contains the mouse button event number. Matching mouse-down and mouse-up events will have the same event number.

case mouseEventClickState

Key to access an integer field that contains the mouse button click state. A click state of 1 represents a single click. A click state of 2 represents a double-click. A click state of 3 represents a triple-click.

case mouseEventPressure

Key to access a double field that contains the mouse button pressure. The pressure value may range from 0 to 1, with 0 representing the mouse being up. This value is commonly set by tablet pens mimicking a mouse.

case mouseEventButtonNumber

Key to access an integer field that contains the mouse button number. For information about the possible values, see CGMouseButton.

case mouseEventDeltaX

Key to access an integer field that contains the horizontal mouse delta since the last mouse movement event.

case mouseEventDeltaY

Key to access an integer field that contains the vertical mouse delta since the last mouse movement event.

case mouseEventInstantMouser

Key to access an integer field. The value is non-zero if the event should be ignored by the Inkwell subsystem.

case mouseEventSubtype

Key to access an integer field that encodes the mouse event subtype as a `kCFNumberIntType`.

case keyboardEventKeycode

Key to access an integer field that contains the virtual keycode of the key-down or key-up event.

case keyboardEventKeyboardType

Key to access an integer field that contains the keyboard type identifier.

case scrollWheelEventDeltaAxis1

Key to access an integer field that contains scrolling data. This field typically contains the change in vertical position since the last scrolling event from a Mighty Mouse scroller or a single-wheel mouse scroller.

case scrollWheelEventDeltaAxis2

Key to access an integer field that contains scrolling data. This field typically contains the change in horizontal position since the last scrolling event from a Mighty Mouse scroller.

case scrollWheelEventDeltaAxis3

This field is not used.

case scrollWheelEventFixedPtDeltaAxis1

Key to access a field that contains scrolling data. The scrolling data represents a line-based or pixel-based change in vertical position since the last scrolling event from a Mighty Mouse scroller or a single-wheel mouse scroller. The scrolling data uses a fixed-point 16.16 signed integer format. For example, if the field contains a value of 1.0, the integer 0x00010000 is returned by `CGEventGetIntegerValueField`. If this key is passed to `CGEventGetDoubleValueField`, the fixed-point value is converted to a double value.

case scrollWheelEventFixedPtDeltaAxis2

Key to access a field that contains scrolling data. The scrolling data represents a line-based or pixel-based change in horizontal position since the last scrolling event from a Mighty Mouse scroller. The scrolling data uses a fixed-point 16.16 signed integer format. For example, if the field contains a value of 1.0, the integer 0x00010000 is returned by `CGEventGetIntegerValueField`. If this key is passed to `CGEventGetDoubleValueField`, the fixed-point value is converted to a double value.

