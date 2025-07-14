

- Core Video
-  CVPixelBufferUnlockBaseAddress(\_:\_:) 

Function

# CVPixelBufferUnlockBaseAddress(\_:\_:)

Unlocks the base address of the pixel buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferUnlockBaseAddress(
    _ pixelBuffer: CVPixelBuffer,
    _ unlockFlags: CVPixelBufferLockFlags
) -> CVReturn
```

## Parameters 

`pixelBuffer`  

The pixel buffer whose base address you want to unlock.

`unlockFlags`  

Either readOnly or `0`; see CVPixelBufferLockFlags for discussion.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

You must call the CVPixelBufferLockBaseAddress(_:_:) function before accessing pixel data with the CPU, and call the CVPixelBufferUnlockBaseAddress(_:_:) function afterward. If you include the readOnly value in the `lockFlags` parameter when locking the buffer, you must also include it when unlocking the buffer.

Important

When accessing pixel data with the GPU, locking is not necessary and can impair performance.

## See Also

### Modifying Pixel Buffers

func CVPixelBufferFillExtendedPixels(CVPixelBuffer) -> CVReturn

Fills the extended pixels of the pixel buffer.

func CVPixelBufferLockBaseAddress(CVPixelBuffer, CVPixelBufferLockFlags) -> CVReturn

Locks the base address of the pixel buffer.

