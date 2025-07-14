

- CarPlay
-  CPMaximumNumberOfGridImages 

Global Variable

# CPMaximumNumberOfGridImages

The maximum number of images that an image row can contain.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
let CPMaximumNumberOfGridImages: Int
```

## Discussion

At runtime, use this value to determine the total number of images that CarPlay allows in an image row. The list item may display fewer images, depending on the width of the vehicle’s primary screen.

## See Also

### Managing Content

var text: String?

The list item’s primary text.

var gridImages: [UIImage]

The images that appear in the list item’s image row.

func update([UIImage])

Adds, removes, reorders, or updates the images in the list item’s image row.

class var maximumImageSize: CGSize

The maximum size of an image that an image row can display.

