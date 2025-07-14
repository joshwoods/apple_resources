

- Quartz
- IKPictureTaker
-  setInputImage(\_:) 

Instance Method

# setInputImage(\_:)

Set the image input for the picture taker.

macOS 10.4+

``` source
@MainActor
func setInputImage(_ image: NSImage!)
```

## Parameters 

`image`  

An `NSImage` object.

## Discussion

The input image is never modified by the picture taker.

## See Also

### Getting and Setting Images

func inputImage() -> NSImage!

Returns the input image associated with the picture taker.

func outputImage() -> NSImage!

Returns the edited image.

