

- Quartz
- IKImageView
-  image() 

Instance Method

# image()

Returns the image associated with the view, after any image corrections.

macOS 10.5+

``` source
@MainActor
func image() -> Unmanaged!
```

## Return Value

The image.

## See Also

### Getting and Setting Images

func setImage(CGImage!, imageProperties: [AnyHashable : Any]!)

Sets the image to display in an image view.

func setImageWith(URL!)

Initializes an image view with the image specified by a URL.

