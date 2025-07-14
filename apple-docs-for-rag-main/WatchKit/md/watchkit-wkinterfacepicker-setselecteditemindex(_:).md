

- WatchKit
- WKInterfacePicker
-  setSelectedItemIndex(\_:) 

Instance Method

# setSelectedItemIndex(\_:)

Selects the specified item in the list.

watchOS 2.0+

``` source
func setSelectedItemIndex(_ itemIndex: Int)
```

## Parameters 

`itemIndex`  

The index of the item to select. This index represents the index into the array of items you set using the setItems(_:) method.

## Discussion

If the value in `itemIndex` exceeds the number of items in the array, the picker selects the last item. If `itemIndex` is negative, the picker selects the first item in the array.

## See Also

### Managing the Picker Contents

func setItems([WKPickerItem]?)

Sets the list of items displayed by the picker.

class WKPickerItem

A single item in a picker interface.

func setCoordinatedAnimations([any WKInterfaceObject &amp; WKImageAnimatable]?)

Sets the interface objects that should coordinate their own animations with the picker.

