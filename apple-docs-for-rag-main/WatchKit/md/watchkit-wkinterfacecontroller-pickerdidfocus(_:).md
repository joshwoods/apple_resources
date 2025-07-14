

- WatchKit
- WKInterfaceController
-  pickerDidFocus(\_:) 

Instance Method

# pickerDidFocus(\_:)

Called to let you know that the specified picker is now receiving input from the Digital Crown.

watchOS 2.0+

``` source
@MainActor
func pickerDidFocus(_ picker: WKInterfacePicker)
```

## Discussion

A picker becomes focused when the user taps it or when you call the focus() method of the picker itself. When a picker is focused, input from the Digital Crown updates the selected item.

The default implementation of this method does nothing. Subclasses can override it and use it to perform actions related to the picker receiving focus. You do not need to call `super` in your implementation.

## See Also

### Managing pickers

func pickerDidResignFocus(WKInterfacePicker)

Called to let you know that the specified picker is no longer receiving input from the Digital Crown.

func pickerDidSettle(WKInterfacePicker)

Called to let you know when the user settles on a value in a picker.

