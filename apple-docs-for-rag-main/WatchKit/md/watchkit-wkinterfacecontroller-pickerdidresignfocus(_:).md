

- WatchKit
- WKInterfaceController
-  pickerDidResignFocus(\_:) 

Instance Method

# pickerDidResignFocus(\_:)

Called to let you know that the specified picker is no longer receiving input from the Digital Crown.

watchOS 2.0+

``` source
@MainActor
func pickerDidResignFocus(_ picker: WKInterfacePicker)
```

## Discussion

The default implementation of this method does nothing. Subclasses can override it and use it to perform actions related to the picker losing focus. You do not need to call `super` in your implementation.

## See Also

### Managing pickers

func pickerDidFocus(WKInterfacePicker)

Called to let you know that the specified picker is now receiving input from the Digital Crown.

func pickerDidSettle(WKInterfacePicker)

Called to let you know when the user settles on a value in a picker.

