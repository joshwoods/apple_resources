

- WatchKit
- WKInterfaceObject
-  setAlpha(\_:) 

Instance Method

# setAlpha(\_:)

Sets the opacity of the interface object.

watchOS 2.0+

``` source
func setAlpha(_ alpha: CGFloat)
```

## Parameters 

`alpha`  

A floating-point number in the range `0.0` to `1.0`, where `0.0` represents totally transparent and `1.0` represents totally opaque.

## Discussion

Use this property to make an object fully or partially transparent. A partially transparent object allows the color or background image associated with the containing group or interface controller show through. A fully transparent object cannot be seen but continues to occupy space in your interface.

Changes to the alpha value of an object are animatable.

## See Also

### Hiding and Showing an Object

func setHidden(Bool)

Hides or shows the interface object in your user interface.

