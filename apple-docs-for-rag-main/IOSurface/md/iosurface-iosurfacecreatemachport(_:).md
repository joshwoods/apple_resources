

- IOSurface
-  IOSurfaceCreateMachPort(\_:) 

Function

# IOSurfaceCreateMachPort(\_:)

Returns a mach_port_t that holds a reference to the IOSurface.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
func IOSurfaceCreateMachPort(_ buffer: IOSurfaceRef) -> mach_port_t
```

## Discussion

This is useful if you need to atomically or securely pass an IOSurface to another task without making the surface global to the entire system. The returned port must be deallocated with mach_port_deallocate or the equivalent.

Note

Any live mach ports created from an IOSurfaceRef implicitly increase the IOSurface’s global use count by one until the port is deleted.

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

func IOSurfaceGetBytesPerRow(IOSurfaceRef) -> Int

Returns the length (in bytes) of each row in a particular buffer.

