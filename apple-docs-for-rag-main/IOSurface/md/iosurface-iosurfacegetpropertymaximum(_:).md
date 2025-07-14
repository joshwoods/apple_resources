

- IOSurface
-  IOSurfaceGetPropertyMaximum(\_:) 

Function

# IOSurfaceGetPropertyMaximum(\_:)

Returns the maximum value for a given property that is guaranteed to be compatible with all of the current devices (GPUs, etc.) in the system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
func IOSurfaceGetPropertyMaximum(_ property: CFString) -> Int
```

## Discussion

The most important values to obtain are:

- `kIOSurfaceBytesPerRow`

- `kIOSurfaceWidth`

- `kIOSurfaceHeight`

- `kIOSurfacePlaneBytesPerRow`

- `kIOSurfacePlaneWidth`

- `kIOSurfacePlaneHeight`

For the width and height properties, the maximum values are the largest that are guaranteed to work for both reading and writing. In OpenGL terms this translates into the largest size that will work for both textures and render targets.

This function returns 0 for properties that have no predefined limit or where the concept of a limit would be considered invalid (such as `kIOSurfacePixelFormat`).

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

