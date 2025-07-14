

- Core Video
-  CVPixelBufferFillExtendedPixels(\_:) 

Function

# CVPixelBufferFillExtendedPixels(\_:)

Fills the extended pixels of the pixel buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferFillExtendedPixels(_ pixelBuffer: CVPixelBuffer) -> CVReturn
```

## Parameters 

`pixelBuffer`  

The pixel buffer whose extended pixels you want to fill.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

This function replicates edge pixels to fill the entire extended region of the image.

## See Also

### Modifying Pixel Buffers

func CVPixelBufferLockBaseAddress(CVPixelBuffer, CVPixelBufferLockFlags) -> CVReturn

Locks the base address of the pixel buffer.

func CVPixelBufferUnlockBaseAddress(CVPixelBuffer, CVPixelBufferLockFlags) -> CVReturn

Unlocks the base address of the pixel buffer.

