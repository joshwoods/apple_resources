

- WatchKit
- WKInterfaceObject
-  setHeight(\_:) 

Instance Method

# setHeight(\_:)

Sets the absolute height (in points) of the object.

watchOS 2.0+

``` source
func setHeight(_ height: CGFloat)
```

## Parameters 

`height`  

The new height of the object. Specifying a value of `0.0` causes the item to have no height.

## Discussion

You cannot use this method to alter the height of tables or the thickness of horizontal separator items. Changing the height of a WKInterfaceImage object causes the image’s content scaling mode to change to UIView.ContentMode.scaleToFill.

Changes to the height of an object are animatable.

## See Also

### Changing an Object’s Size

func setWidth(CGFloat)

Sets the absolute width (in points) of the object.

func setRelativeWidth(CGFloat, withAdjustment: CGFloat)

Sets the width of the object relative to its container.

func setRelativeHeight(CGFloat, withAdjustment: CGFloat)

Sets the height of the object relative to its container.

func sizeToFitWidth()

Sets the width of the object to fit its current content.

func sizeToFitHeight()

Sets the height of the object so that it fills the available vertical space.

