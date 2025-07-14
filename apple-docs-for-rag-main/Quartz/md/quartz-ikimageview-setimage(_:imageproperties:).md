

- Quartz
- IKImageView
-  setImage(\_:imageProperties:) 

Instance Method

# setImage(\_:imageProperties:)

Sets the image to display in an image view.

macOS 10.5+

``` source
@MainActor
func setImage(
    _ image: CGImage!,
    imageProperties metaData: [AnyHashable : Any]!
)
```

## Parameters 

`image`  

The image to set.

`metaData`  

A dictionary that contains metadata that describes the image.

## See Also

### Related Documentation

func imageProperties() -> [AnyHashable : Any]!

Returns the metadata for the image in the view.

### Getting and Setting Images

func image() -> Unmanaged&lt;CGImage>!

Returns the image associated with the view, after any image corrections.

func setImageWith(URL!)

Initializes an image view with the image specified by a URL.

