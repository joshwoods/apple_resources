

- CarPlay
- CPListImageRowItem
-  update(\_:) 

Instance Method

# update(\_:)

Adds, removes, reorders, or updates the images in the list item’s image row.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func update(_ gridImages: [UIImage])
```

## Parameters 

`gridImages`  

An array of images to display in the list item’s image row.

## Discussion

This method is multipurpose. Use it to add new images to the image row, and to remove or reorder existing images.

Provide images that are display-ready. If necessary, provide light and dark variants of each image using an asset catalog, or use instances of UIImageAsset and register an image for each interface style.

To properly size your images, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size that CarPlay allows for an image, and CPMaximumNumberOfGridImages to establish the total number of images that an image row can display. The list item may display fewer images, depending on the width of the vehicle’s primary screen.

CarPlay doesn’t support animated images. If you provide animated images, CarPlay uses only the first image in each animation sequence.

## See Also

### Managing Content

var text: String?

The list item’s primary text.

var gridImages: [UIImage]

The images that appear in the list item’s image row.

class var maximumImageSize: CGSize

The maximum size of an image that an image row can display.

let CPMaximumNumberOfGridImages: Int

The maximum number of images that an image row can contain.

