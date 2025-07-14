

- Core Video
-  CVImageBufferGetColorSpace(\_:) 

Function

# CVImageBufferGetColorSpace(\_:)

Returns the color space of a Core Video image buffer.

macOS 10.4+

``` source
func CVImageBufferGetColorSpace(_ imageBuffer: CVImageBuffer) -> Unmanaged?
```

## Parameters 

`imageBuffer`  

The image buffer containing the color space to retrieve.

## Return Value

The color space of the image buffer, or nil if you pass a value for the image buffer that isn’t a CVImageBuffer type.

## See Also

### Inspecting image buffers

func CVImageBufferGetCleanRect(CVImageBuffer) -> CGRect

Returns the source rectangle of a Core Video image buffer that represents the clean aperture of the buffer in encoded pixels.

func CVImageBufferGetDisplaySize(CVImageBuffer) -> CGSize

Returns the nominal output display size, in square pixels, of a Core Video image buffer.

func CVImageBufferGetEncodedSize(CVImageBuffer) -> CGSize

Returns the full encoded dimensions of a Core Video image buffer.

func CVImageBufferIsFlipped(CVImageBuffer) -> Bool

Returns a Boolean value indicating whether the image is vertically flipped.

