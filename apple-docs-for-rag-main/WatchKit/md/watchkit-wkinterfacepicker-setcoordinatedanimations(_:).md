

- WatchKit
- WKInterfacePicker
-  setCoordinatedAnimations(\_:) 

Instance Method

# setCoordinatedAnimations(\_:)

Sets the interface objects that should coordinate their own animations with the picker.

watchOS 2.0+

``` source
func setCoordinatedAnimations(_ coordinatedAnimations: [any WKInterfaceObject & WKImageAnimatable]?)
```

## Parameters 

`coordinatedAnimations`  

An array of objects that conform to the WKImageAnimatable protocol. The objects in this array should be displaying an animated image. Specify `nil` to remove all coordinated objects from the picker.

## Discussion

Use this method to link other animatable images to the picker. When the user turns the crown, the picker updates the currently displayed image in each of the linked interface objects.

The animated images associated with the interface objects may have any number of frames. For each object, the picker determines the appropriate image to display based on the percentage offset from the beginning of the picker’s own item list. The first picker item displays the first image in the animated sequence and the last picker item displays the last item. If the picker has ten items and an animated image has 20 images, each new picker item advances the animated image by two frames.

## See Also

### Managing the Picker Contents

func setItems([WKPickerItem]?)

Sets the list of items displayed by the picker.

class WKPickerItem

A single item in a picker interface.

func setSelectedItemIndex(Int)

Selects the specified item in the list.

