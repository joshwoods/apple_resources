

- TV Services
- TVTopShelfItem
-  imageURL(for:) 

Instance Method

# imageURL(for:)

Returns an image associated with the current item.

tvOS 13.0+

``` source
func imageURL(for traits: TVTopShelfItem.ImageTraits) -> URL?
```

## Parameters 

`traits`  

The traits that describe the image.

## Return Value

The image associated with the specified traits; otherwise, `nil` if you did not previously assign an image with the specified traits.

## See Also

### Providing an Image for the Item

func setImageURL(URL?, for: TVTopShelfItem.ImageTraits)

Associates an image with the current item.

struct ImageTraits

Constants describing the image format.

