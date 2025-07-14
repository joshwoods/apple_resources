

- Quartz
- IKPictureTaker
-  inputImage() 

Instance Method

# inputImage()

Returns the input image associated with the picture taker.

macOS 10.4+

``` source
@MainActor
func inputImage() -> NSImage!
```

## Return Value

The input image.

## Discussion

The input image is never modified by the picture taker.

## See Also

### Getting and Setting Images

func setInputImage(NSImage!)

Set the image input for the picture taker.

func outputImage() -> NSImage!

Returns the edited image.

