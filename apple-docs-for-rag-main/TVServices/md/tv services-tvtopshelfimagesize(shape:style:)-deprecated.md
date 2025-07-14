

- TV Services
-  TVTopShelfImageSize(shape:style:) Deprecated

Function

# TVTopShelfImageSize(shape:style:)

Returns the ideal size for an image, according to its particular shape and style.

tvOS 9.0–13.0Deprecated

``` source
func TVTopShelfImageSize(
    shape: TVContentItemImageShape,
    style: TVTopShelfContentStyle
) -> CGSize
```

Deprecated

TVTopShelfImageSizeForShape has been replaced by \[TVTopShelfSectionedContent imageSizeForImageShape:\] and \[TVTopShelfInsetContent imageSize\]

## Parameters 

`shape`  

The shape of the content item.

`style`  

The style of the TV Top Shelf user interface.

## Discussion

Call this function to determine the ideal image size to use to avoid image scaling. Typically, if your app has access to multiple images for a given piece of content, you use this function to choose which image most closely matches the ideal size for the version of the operating system that your app is running on. An image provided in that size does not require any image scaling. If you request the size of a shape that is not allowed in the given style, the function returns CGSizeZero.

## See Also

### Content

class TVContentItem

An object that describes either a piece of content or a container for other content items.

Deprecated

class TVContentIdentifier

An object that uniquely identifies media content in either a single piece or a collection.

Deprecated

