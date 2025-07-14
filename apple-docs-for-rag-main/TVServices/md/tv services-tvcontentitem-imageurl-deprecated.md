

- TV Services
- TVContentItem
-  imageURL Deprecated

Instance Property

# imageURL

A URL giving the location of the image to be displayed for this content item.

tvOS 9.0–11.0Deprecated

``` source
var imageURL: URL? { get set }
```

Deprecated

Use setImageURL:forTraits: to set image URLs into TVContentItem.

## Discussion

The image URL can be an absolute path on the local device or an HTTP path. The preferred file format for this image is a layered image file that provides the proper 3d effects. For more information, see App Programming Guide for tvOS.

## See Also

### Accessing Image Resources

func imageURL(forTraits: TVContentItemImageTrait) -> URL?

Retrieve the URL for the image that best matches the specified traits.

Deprecated

func setImageURL(URL?, forTraits: TVContentItemImageTrait)Deprecated

struct TVContentItemImageTrait

Traits describing the type of image you want.

