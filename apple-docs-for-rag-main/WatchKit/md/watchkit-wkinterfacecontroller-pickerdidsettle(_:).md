

- WatchKit
- WKInterfaceController
-  pickerDidSettle(\_:) 

Instance Method

# pickerDidSettle(\_:)

Called to let you know when the user settles on a value in a picker.

watchOS 2.0+

``` source
@MainActor
func pickerDidSettle(_ picker: WKInterfacePicker)
```

## Parameters 

`picker`  

The picker containing the selected value.

## Discussion

Use this method to perform any expensive operations associated with selecting a picker item. The user can turn the Digital Crown quickly to scroll through the items in the picker. This method is called only after scrolling subsides and the value remains steady for a reasonable period of time. For inexpensive operations, you can continue to use the picker’s action method, which is called for each change of the selected item.

The default implementation of this method does nothing. Subclasses can override it and use it to perform actions related to the picker settling on a value. You do not need to call `super` in your implementation.

## See Also

### Managing pickers

func pickerDidFocus(WKInterfacePicker)

Called to let you know that the specified picker is now receiving input from the Digital Crown.

func pickerDidResignFocus(WKInterfacePicker)

Called to let you know that the specified picker is no longer receiving input from the Digital Crown.

