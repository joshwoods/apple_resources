

- Core Video
-  CVImageBufferIsFlipped(\_:) 

Function

# CVImageBufferIsFlipped(\_:)

Returns a Boolean value indicating whether the image is vertically flipped.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVImageBufferIsFlipped(_ imageBuffer: CVImageBuffer) -> Bool
```

## Parameters 

`imageBuffer`  

An image buffer.

## Return Value

Returns true if `{0,0}` represents the upper left of the image, or false if `{0,0}` represents the lower left of the image.

## See Also

### Inspecting image buffers

func CVImageBufferGetCleanRect(CVImageBuffer) -> CGRect

Returns the source rectangle of a Core Video image buffer that represents the clean aperture of the buffer in encoded pixels.

func CVImageBufferGetColorSpace(CVImageBuffer) -> Unmanaged&lt;CGColorSpace>?

Returns the color space of a Core Video image buffer.

func CVImageBufferGetDisplaySize(CVImageBuffer) -> CGSize

Returns the nominal output display size, in square pixels, of a Core Video image buffer.

func CVImageBufferGetEncodedSize(CVImageBuffer) -> CGSize

Returns the full encoded dimensions of a Core Video image buffer.

