

- WatchKit
- WKInterfaceObject
-  setRelativeWidth(\_:withAdjustment:) 

Instance Method

# setRelativeWidth(\_:withAdjustment:)

Sets the width of the object relative to its container.

watchOS 2.0+

``` source
func setRelativeWidth(
    _ width: CGFloat,
    withAdjustment adjustment: CGFloat
)
```

## Parameters 

`width`  

The width of the object relative to its immediate container. This value represents the percentage of the container’s width. This value must be between `0.0` and `1.0`, and values outside of that range are clamped to the minimum or maximum value.

`adjustment`  

The amount (in points) to add or subtract from the relative width. Positive values increase the width of the item and negative values decrease it.

## Discussion

You cannot use this method to alter the height of tables or separator items. Changes to the width of an object are animatable.

## See Also

### Changing an Object’s Size

func setWidth(CGFloat)

Sets the absolute width (in points) of the object.

func setHeight(CGFloat)

Sets the absolute height (in points) of the object.

func setRelativeHeight(CGFloat, withAdjustment: CGFloat)

Sets the height of the object relative to its container.

func sizeToFitWidth()

Sets the width of the object to fit its current content.

func sizeToFitHeight()

Sets the height of the object so that it fills the available vertical space.

