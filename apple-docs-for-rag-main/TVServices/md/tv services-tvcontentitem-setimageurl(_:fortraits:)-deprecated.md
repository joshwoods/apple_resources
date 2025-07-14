

- TV Services
- TVContentItem
-  setImageURL(\_:forTraits:) Deprecated

Instance Method

# setImageURL(\_:forTraits:)

tvOS 11.0–13.0Deprecated

``` source
func setImageURL(
    _ aURL: URL?,
    forTraits traits: TVContentItemImageTrait
)
```

## Parameters 

`aURL`  

The URL corresponding to the image location. This parameter can be an absolute path on the local device or an HTTP path. Specify `nil` to remove the image associated with the given traits.

`traits`  

The traits to associate with the image. For example, you might specify that the image applies only to dark interfaces.

## Discussion

The preferred file format for this image is a layered image file that provides the proper 3d effects. For more information, see App Programming Guide for tvOS.

## See Also

### Accessing Image Resources

var imageURL: URL?

A URL giving the location of the image to be displayed for this content item.

Deprecated

func imageURL(forTraits: TVContentItemImageTrait) -> URL?

Retrieve the URL for the image that best matches the specified traits.

Deprecated

struct TVContentItemImageTrait

Traits describing the type of image you want.

