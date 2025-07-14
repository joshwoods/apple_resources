

- IOSurface
-  kIOSurfaceOffset 

Global Variable

# kIOSurfaceOffset

CFNumber for the starting offset into the buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
let kIOSurfaceOffset: CFString
```

## Discussion

Defaults to 0.

## See Also

### Constants

let kIOSurfaceAllocSize: CFString

CFNumber of the total allocation size of the buffer including all planes.

let kIOSurfaceBytesPerElement: CFString

CFNumber for the total number of bytes in an element.

let kIOSurfaceBytesPerRow: CFString

CFNumber for the bytes per row of the buffer.

let kIOSurfaceCacheMode: CFString

CFNumber for the CPU cache mode to be used for the allocation.

let kIOSurfaceColorSpace: CFString

let kIOSurfaceElementHeight: CFString

CFNumber for how many pixels high each element is.

let kIOSurfaceElementWidth: CFString

CFNumber for how many pixels wide each element is.

let kIOSurfaceHeight: CFString

CFNumber for the height of the IOSurface buffer in pixels.

let kIOSurfaceICCProfile: CFString

let kIOSurfaceIsGlobal: CFString

CFBoolean If true, the IOSurface may be looked up by any task in the system by its ID.

Deprecated

let kIOSurfaceName: CFString

let kIOSurfacePixelFormat: CFString

A 32-bit unsigned integer doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd that stores the traditional macOS buffer format.

let kIOSurfacePixelSizeCastingAllowed: CFString

let kIOSurfacePlaneBase: CFString

CFNumber for the base offset into the buffer for this plane.

let kIOSurfacePlaneBitsPerElement: CFString

