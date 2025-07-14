

- IOSurface
-  IOSurface Constants 

API Collection

# IOSurface Constants

## Topics

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

let kIOSurfaceOffset: CFString

CFNumber for the starting offset into the buffer.

let kIOSurfacePixelFormat: CFString

A 32-bit unsigned integer doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd that stores the traditional macOS buffer format.

let kIOSurfacePixelSizeCastingAllowed: CFString

let kIOSurfacePlaneBase: CFString

CFNumber for the base offset into the buffer for this plane.

let kIOSurfacePlaneBitsPerElement: CFString

let kIOSurfacePlaneBytesPerElement: CFString

CFNumber for the bytes per element of this plane.

let kIOSurfacePlaneBytesPerRow: CFString

CFNumber for the bytes per row of this plane.

let kIOSurfacePlaneComponentBitDepths: CFString

let kIOSurfacePlaneComponentBitOffsets: CFString

let kIOSurfacePlaneComponentNames: CFString

let kIOSurfacePlaneComponentRanges: CFString

let kIOSurfacePlaneComponentTypes: CFString

let kIOSurfacePlaneElementHeight: CFString

CFNumber for the element height of this plane.

let kIOSurfacePlaneElementWidth: CFString

CFNumber for the element width of this plane.

let kIOSurfacePlaneHeight: CFString

CFNumber for the height of this plane in pixels.

let kIOSurfacePlaneInfo: CFString

CFArray describing each image plane in the buffer as a CFDictionary.

let kIOSurfacePlaneOffset: CFString

CFNumber for the offset into the buffer for this plane.

let kIOSurfacePlaneSize: CFString

CFNumber for the total data size of this plane.

let kIOSurfacePlaneWidth: CFString

CFNumber for the width of this plane in pixels.

let kIOSurfaceSubsampling: CFString

var kIOSurfaceSuccess: Int32

let kIOSurfaceWidth: CFString

CFNumber for the width of the IOSurface buffer in pixels.

## See Also

### Reference

IOSurface Structures

IOSurface Functions

