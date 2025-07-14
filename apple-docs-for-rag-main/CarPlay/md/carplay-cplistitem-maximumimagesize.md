

- CarPlay
- CPListItem
-  maximumImageSize 

Type Property

# maximumImageSize

The maximum size of a list item’s image and accessory image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class var maximumImageSize: CGSize { get }
```

## Discussion

At runtime, use this value to determine the maximum size for a list item’s image and accessory image.

## See Also

### Managing Content

var text: String?

The list item’s primary text.

func setText(String)

Updates the list item’s primary text.

var detailText: String?

The list item’s secondary text.

func setDetailText(String?)

Updates the list item’s secondary text.

var image: UIImage?

The image that the list item displays in its leading region.

func setImage(UIImage?)

Updates the list item’s image.

