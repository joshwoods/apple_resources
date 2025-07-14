

- WatchKit
- WKInterfaceGroup
-  setContentInset(\_:) 

Instance Method

# setContentInset(\_:)

Sets the distance between the edges of the group and any contained objects.

watchOS 2.0+

``` source
func setContentInset(_ contentInset: UIEdgeInsets)
```

## Parameters 

`contentInset`  

The insets to apply to contained objects. All inset values are measured in points. Inset values must not be less than `0`.

## Discussion

Use this method to change the default insets you set in Interface Builder. Changes to the content insets of a group are animatable.

## See Also

### Setting the Layout Information

func setCornerRadius(CGFloat)

Changes the radius to use when drawing rounded corners for the group.

