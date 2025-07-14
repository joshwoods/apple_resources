

- CarPlay
- CPListImageRowItem
-  init(text:images:imageTitles:) 

Initializer

# init(text:images:imageTitles:)

Creates a list item that displays a row of images with a title below each image.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
init(
    text: String,
    images: [UIImage],
    imageTitles: [String]
)
```

## Parameters 

`text`  

The list item’s primary text.

`images`  

An array of images to display in the list item’s image row.

`imageTitles`  

An array of strings that represent the image titles.

## Discussion

Provide images that are display-ready. If necessary, provide light and dark variants of each image using an asset catalog, or use instances of UIImageAsset and register an image for each interface style.

To properly size your images, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size that CarPlay allows for an image, and CPMaximumNumberOfGridImages to establish the total number of images that an image row can display. The list item may display fewer images, depending on the width of the vehicle’s primary screen.

Carplay uses `UIImageAsset` to combine multiple UIImage objects with different trait collections into a single `UIImage` and the framework resizes images, if necessary. CarPlay doesn’t support animated images, if you provide animated images, the framework uses only the first image in each animation sequence.

The number of titles in the `imageTitles` list needs to be equal to the number of images in the `images`.

## See Also

### Creating a List Image Row Item

init(text: String, images: [UIImage])

Creates a list item that displays a row of images.

