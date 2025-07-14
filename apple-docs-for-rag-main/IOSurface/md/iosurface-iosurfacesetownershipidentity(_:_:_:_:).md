

- IOSurface
-  IOSurfaceSetOwnershipIdentity(\_:\_:\_:\_:) 

Function

# IOSurfaceSetOwnershipIdentity(\_:\_:\_:\_:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
func IOSurfaceSetOwnershipIdentity(
    _ buffer: IOSurfaceRef,
    _ task_id_token: task_id_token_t,
    _ newLedgerTag: Int32,
    _ newLedgerOptions: UInt32
) -> kern_return_t
```

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

