

- Video Toolbox
-  VTPixelRotationSessionCreate(\_:\_:) 

Function

# VTPixelRotationSessionCreate(\_:\_:)

Creates a session to rotate images between pixel buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func VTPixelRotationSessionCreate(
    _ allocator: CFAllocator?,
    _ pixelRotationSessionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the session. Specify `NULL` to use the default allocator.

`pixelRotationSessionOut`  

On output, an initialized pixel rotation session.

## See Also

### Managing a Session

func VTPixelRotationSessionInvalidate(VTPixelRotationSession)

Tears down a pixel rotation session.

