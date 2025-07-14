

- TV Services
- TVContentItem
-  imageURL(forTraits:) Deprecated

Instance Method

# imageURL(forTraits:)

Retrieve the URL for the image that best matches the specified traits.

tvOS 11.0–13.0Deprecated

``` source
func imageURL(forTraits traits: TVContentItemImageTrait) -> URL?
```

## Parameters 

`traits`  

The traits for the image you want. For example, you might ask specifically for the variant of the image that supports a dark interface.

## Return Value

The URL for the image asset, or `nil` if an image with the specified traits was not found.

## Discussion

The image URL can be an absolute path on the local device or an HTTP path. The preferred file format for this image is a layered image file that provides the proper 3d effects. For more information, see App Programming Guide for tvOS.

## See Also

### Accessing Image Resources

var imageURL: URL?

A URL giving the location of the image to be displayed for this content item.

Deprecated

func setImageURL(URL?, forTraits: TVContentItemImageTrait)Deprecated

struct TVContentItemImageTrait

Traits describing the type of image you want.

