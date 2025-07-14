

- IOSurface
-  kIOSurfaceIsGlobal Deprecated

Global Variable

# kIOSurfaceIsGlobal

CFBoolean If true, the IOSurface may be looked up by any task in the system by its ID.

iOS 11.0–11.0DeprecatediPadOS 11.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.11DeprecatedtvOS 11.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let kIOSurfaceIsGlobal: CFString
```

Deprecated

Global surfaces are insecure

## Discussion

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

let kIOSurfaceName: CFString

let kIOSurfaceOffset: CFString

CFNumber for the starting offset into the buffer.

let kIOSurfacePixelFormat: CFString

A 32-bit unsigned integer doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd that stores the traditional macOS buffer format.

let kIOSurfacePixelSizeCastingAllowed: CFString

let kIOSurfacePlaneBase: CFString

CFNumber for the base offset into the buffer for this plane.

let kIOSurfacePlaneBitsPerElement: CFString

