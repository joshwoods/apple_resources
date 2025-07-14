

- Core Video
-  CVImageBufferGetEncodedSize(\_:) 

Function

# CVImageBufferGetEncodedSize(\_:)

Returns the full encoded dimensions of a Core Video image buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVImageBufferGetEncodedSize(_ imageBuffer: CVImageBuffer) -> CGSize
```

## Parameters 

`imageBuffer`  

The image buffer containing the encoded size to retrieve.

## Return Value

A CGSize structure defining the full encoded size of the image buffer. The size is zero if you pass a value for the image buffer that isn’t a CVImageBuffer type.

## Discussion

For example, for an NTSC DV frame, this function returns an encoded size of 720 x 480. When you create a CIImage object from a Core Video image buffer, use this call to retrieve the image size.

## See Also

### Inspecting image buffers

func CVImageBufferGetCleanRect(CVImageBuffer) -> CGRect

Returns the source rectangle of a Core Video image buffer that represents the clean aperture of the buffer in encoded pixels.

func CVImageBufferGetColorSpace(CVImageBuffer) -> Unmanaged&lt;CGColorSpace>?

Returns the color space of a Core Video image buffer.

func CVImageBufferGetDisplaySize(CVImageBuffer) -> CGSize

Returns the nominal output display size, in square pixels, of a Core Video image buffer.

func CVImageBufferIsFlipped(CVImageBuffer) -> Bool

Returns a Boolean value indicating whether the image is vertically flipped.

