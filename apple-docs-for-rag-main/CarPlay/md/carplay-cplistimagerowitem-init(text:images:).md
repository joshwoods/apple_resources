

- CarPlay
- CPListImageRowItem
-  init(text:images:) 

Initializer

# init(text:images:)

Creates a list item that displays a row of images.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    text: String,
    images: [UIImage]
)
```

## Parameters 

`text`  

The list item’s primary text.

`images`  

An array of images to display in the list item’s image row.

## Discussion

Provide images that are display-ready. If necessary, provide light and dark variants of each image using an asset catalog, or use instances of UIImageAsset and register an image for each interface style.

To properly size your images, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size that CarPlay allows for an image, and CPMaximumNumberOfGridImages to establish the total number of images that an image row can display. The list item may display fewer images, depending on the width of the vehicle’s primary screen.

CarPlay doesn’t support animated images. If you provide animated images, CarPlay uses only the first image in each animation sequence.

## See Also

### Creating a List Image Row Item

init(text: String, images: [UIImage], imageTitles: [String])

Creates a list item that displays a row of images with a title below each image.

