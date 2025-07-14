

- Quartz
- IKImageView
-  setImageWith(\_:) 

Instance Method

# setImageWith(\_:)

Initializes an image view with the image specified by a URL.

macOS 10.5+

``` source
@MainActor
func setImageWith(_ url: URL!)
```

## Parameters 

`url`  

The URL that specifies the location of the image.

## Discussion

This method is the preferred initializer for RAW images. If you use this method for a TIFF file that contains multiple images, only the first image is displayed.

## See Also

### Getting and Setting Images

func image() -> Unmanaged&lt;CGImage>!

Returns the image associated with the view, after any image corrections.

func setImage(CGImage!, imageProperties: [AnyHashable : Any]!)

Sets the image to display in an image view.

