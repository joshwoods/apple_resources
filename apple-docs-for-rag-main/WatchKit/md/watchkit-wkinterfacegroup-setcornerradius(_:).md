

- WatchKit
- WKInterfaceGroup
-  setCornerRadius(\_:) 

Instance Method

# setCornerRadius(\_:)

Changes the radius to use when drawing rounded corners for the group.

watchOS 2.0+

``` source
func setCornerRadius(_ cornerRadius: CGFloat)
```

## Parameters 

`cornerRadius`  

The radius (in points) of the circle used to round the corners of the groups edges.

## Discussion

Setting the radius to a value greater than `0.0` causes the group to draw rounded corners on its background. When a corner radius is applied, the group’s background color or image are clipped accordingly.

The default corner radius for groups is 6 points.

## See Also

### Setting the Layout Information

func setContentInset(UIEdgeInsets)

Sets the distance between the edges of the group and any contained objects.

