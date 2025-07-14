

- WatchKit
- WKInterfacePicker
-  setItems(\_:) 

Instance Method

# setItems(\_:)

Sets the list of items displayed by the picker.

watchOS 2.0+

``` source
func setItems(_ items: [WKPickerItem]?)
```

## Parameters 

`items`  

An array of WKPickerItem objects. Each item in the array represents a single selectable item.

## Discussion

The items you specify must be configured appropriate for the picker style. For example, items displayed using the list style must contain a title. The picker displays items in the order they appear in the `items` array. When a selection occurs, the picker reports the index of the selected item to its associated action method.

This method displays the new items in the picker right away. If the previously specified selection index exceeds the number of items in the new array, the picker selects the last item in the array.

## See Also

### Managing the Picker Contents

class WKPickerItem

A single item in a picker interface.

func setSelectedItemIndex(Int)

Selects the specified item in the list.

func setCoordinatedAnimations([any WKInterfaceObject &amp; WKImageAnimatable]?)

Sets the interface objects that should coordinate their own animations with the picker.

