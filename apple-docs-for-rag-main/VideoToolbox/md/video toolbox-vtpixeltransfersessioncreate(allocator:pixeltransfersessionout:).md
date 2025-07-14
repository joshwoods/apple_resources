

- Video Toolbox
-  VTPixelTransferSessionCreate(allocator:pixelTransferSessionOut:) 

Function

# VTPixelTransferSessionCreate(allocator:pixelTransferSessionOut:)

Creates a session for transferring images between Core Video image buffers that hold pixels in main memory.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.8+tvOS 16.0+visionOS 1.0+

``` source
func VTPixelTransferSessionCreate(
    allocator: CFAllocator?,
    pixelTransferSessionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the session. Pass `NULL` to use the default allocator.

`pixelTransferSessionOut`  

Points to a variable to receive the new pixel transfer session.

## Discussion

The function creates a session for transferring images between CVPixelBuffer objects.

