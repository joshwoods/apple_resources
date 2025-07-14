

- Compositor Services
- AxisDirectionConvention
-  AxisDirectionConvention.rightUpBack 

Case

# AxisDirectionConvention.rightUpBack

The convention that uses a counterclockwise winding order and positions the leading pixel at the top-left corner of the view.

visionOS 2.0+

``` source
case rightUpBack
```

## Discussion

This convention positions the left-most pixel at the left edge of the view and the top-most pixel at the top edge of the view, and the system renders with a counterclockwise winding order.

## See Also

### Getting the axis directions

case rightUpForward

The convention that uses a clockwise winding order and positions the leading pixel at the top-left corner of the view.

case rightDownBack

The convention that uses a counterclockwise winding order and positions the leading pixel at the bottom-left corner of the view.

case rightDownForward

The convention that uses a clockwise winding order and positions the leading pixel at the bottom-left corner of the view.

