

- CarPlay
- CPListImageRowItem
-  maximumImageSize 

Type Property

# maximumImageSize

The maximum size of an image that an image row can display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class var maximumImageSize: CGSize { get }
```

## Discussion

At runtime, use this value to determine the maximum size that CarPlay allows for a single image in an image row.

## See Also

### Managing Content

var text: String?

The list item’s primary text.

var gridImages: [UIImage]

The images that appear in the list item’s image row.

func update([UIImage])

Adds, removes, reorders, or updates the images in the list item’s image row.

let CPMaximumNumberOfGridImages: Int

The maximum number of images that an image row can contain.

