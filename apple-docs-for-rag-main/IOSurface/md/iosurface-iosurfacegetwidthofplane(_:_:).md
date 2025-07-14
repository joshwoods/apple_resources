

- IOSurface
-  IOSurfaceGetWidthOfPlane(\_:\_:) 

Function

# IOSurfaceGetWidthOfPlane(\_:\_:)

Returns the width of the specified plane (in pixels).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
func IOSurfaceGetWidthOfPlane(
    _ buffer: IOSurfaceRef,
    _ planeIndex: Int
) -> Int
```

## Discussion

If the planeIndex is greater than or equal to the plane count of the IOSurface, zero is returned…. with one exception. If this IOSurface has zero planes and a planeIndex of zero is passed in, the routines function just like the non-planar APIs. This is to allow higher level code to treat planar and non-planar buffers is a more uniform fashion.

## See Also

### Functions

func IOSurfaceAlignProperty(CFString, Int) -> Int

Returns the smallest aligned value greater than or equal to the specified value.

func IOSurfaceAllowsPixelSizeCasting(IOSurfaceRef) -> Bool

func IOSurfaceCopyAllValues(IOSurfaceRef) -> CFDictionary?

func IOSurfaceCopyValue(IOSurfaceRef, CFString) -> CFTypeRef?

Retrieves a value from the dictionary associated with the buffer.

func IOSurfaceCreate(CFDictionary) -> IOSurfaceRef?

Creates a brand new IOSurface object

func IOSurfaceCreateMachPort(IOSurfaceRef) -> mach_port_t

Returns a mach_port_t that holds a reference to the IOSurface.

func IOSurfaceCreateXPCObject(IOSurfaceRef) -> xpc_object_t

Returns an xpc_object_t that holds a reference to the IOSurface.

func IOSurfaceDecrementUseCount(IOSurfaceRef)

Decrements the per-process usage count for an IOSurface.

func IOSurfaceGetAllocSize(IOSurfaceRef) -> Int

Returns the total allocation size of the buffer including all planes.

func IOSurfaceGetBaseAddress(IOSurfaceRef) -> UnsafeMutableRawPointer

Returns the address of the first byte of data in a particular buffer.

func IOSurfaceGetBaseAddressOfPlane(IOSurfaceRef, Int) -> UnsafeMutableRawPointer

Returns the address of the first byte of data in the specified plane.

func IOSurfaceGetBitDepthOfComponentOfPlane(IOSurfaceRef, Int, Int) -> Int

func IOSurfaceGetBitOffsetOfComponentOfPlane(IOSurfaceRef, Int, Int) -> Int

func IOSurfaceGetBytesPerElement(IOSurfaceRef) -> Int

Returns the length (in bytes) of each element in a particular buffer.

func IOSurfaceGetBytesPerElementOfPlane(IOSurfaceRef, Int) -> Int

Returns the size of each element (in bytes) in the specified plane.

