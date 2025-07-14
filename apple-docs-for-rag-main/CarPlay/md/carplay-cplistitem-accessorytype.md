

- CarPlay
- CPListItem
-  accessoryType 

Instance Property

# accessoryType

The accessory that the list item displays in its trailing region.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var accessoryType: CPListItemAccessoryType { get set }
```

## Discussion

If you update the list item to display an accessory image using the setAccessoryImage(_:) method, CarPlay sets this property’s value to CPListItemAccessoryType.none.

## See Also

### Managing Accessories

enum CPListItemAccessoryType

The accessory types that a list item can display.

var accessoryImage: UIImage?

The image that the list item displays in its trailing region.

func setAccessoryImage(UIImage?)

Updates the list item’s accessory image.

