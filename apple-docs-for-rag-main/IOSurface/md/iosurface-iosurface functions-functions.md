

- IOSurface
-  IOSurface Functions 

API Collection

# IOSurface Functions

## Topics

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

func IOSurfaceGetBytesPerRow(IOSurfaceRef) -> Int

Returns the length (in bytes) of each row in a particular buffer.

func IOSurfaceGetBytesPerRowOfPlane(IOSurfaceRef, Int) -> Int

Returns the size of each row (in bytes) in the specified plane.

func IOSurfaceGetElementHeight(IOSurfaceRef) -> Int

Returns the height (in pixels) of each element in a particular buffer.

func IOSurfaceGetElementHeightOfPlane(IOSurfaceRef, Int) -> Int

Returns the height (in pixels) of each element in the specified plane.

func IOSurfaceGetElementWidth(IOSurfaceRef) -> Int

Returns the width (in pixels) of each element in a particular buffer.

func IOSurfaceGetElementWidthOfPlane(IOSurfaceRef, Int) -> Int

Returns the width (in pixels) of each element in the specified plane.

func IOSurfaceGetHeight(IOSurfaceRef) -> Int

Returns the height of the IOSurface buffer in pixels.

func IOSurfaceGetHeightOfPlane(IOSurfaceRef, Int) -> Int

Returns the height of the specified plane (in pixels).

func IOSurfaceGetID(IOSurfaceRef) -> IOSurfaceID

Retrieves the unique IOSurfaceID value for an IOSurface.

func IOSurfaceGetNameOfComponentOfPlane(IOSurfaceRef, Int, Int) -> IOSurfaceComponentName

func IOSurfaceGetNumberOfComponentsOfPlane(IOSurfaceRef, Int) -> Int

func IOSurfaceGetPixelFormat(IOSurfaceRef) -> OSType

Returns an unsigned integer that contains the traditional macOS buffer format.

func IOSurfaceGetPlaneCount(IOSurfaceRef) -> Int

func IOSurfaceGetPropertyAlignment(CFString) -> Int

Returns the alignment requirements for a property (if any).

func IOSurfaceGetPropertyMaximum(CFString) -> Int

Returns the maximum value for a given property that is guaranteed to be compatible with all of the current devices (GPUs, etc.) in the system.

func IOSurfaceGetRangeOfComponentOfPlane(IOSurfaceRef, Int, Int) -> IOSurfaceComponentRange

func IOSurfaceGetSeed(IOSurfaceRef) -> UInt32

func IOSurfaceGetSubsampling(IOSurfaceRef) -> IOSurfaceSubsampling

func IOSurfaceGetTypeID() -> CFTypeID

func IOSurfaceGetTypeOfComponentOfPlane(IOSurfaceRef, Int, Int) -> IOSurfaceComponentType

func IOSurfaceGetUseCount(IOSurfaceRef) -> Int32

Returns the per-process usage count for an IOSurface.

func IOSurfaceGetWidth(IOSurfaceRef) -> Int

Returns the width of the IOSurface buffer in pixels.

func IOSurfaceGetWidthOfPlane(IOSurfaceRef, Int) -> Int

Returns the width of the specified plane (in pixels).

func IOSurfaceIncrementUseCount(IOSurfaceRef)

Increments the per-process usage count for an IOSurface.

func IOSurfaceIsInUse(IOSurfaceRef) -> Bool

Returns true of an IOSurface is in use by any process in the system, otherwise false.

func IOSurfaceLock(IOSurfaceRef, IOSurfaceLockOptions, UnsafeMutablePointer&lt;UInt32>?) -> kern_return_t

“Lock” an IOSurface for reading or writing.

func IOSurfaceLookup(IOSurfaceID) -> IOSurfaceRef?

Performs an atomic lookup and retain of an IOSurface by its IOSurfaceID.

func IOSurfaceLookupFromMachPort(mach_port_t) -> IOSurfaceRef?

Recreates an IOSurfaceRef from a mach port.

func IOSurfaceLookupFromXPCObject(xpc_object_t) -> IOSurfaceRef?

func IOSurfaceRemoveAllValues(IOSurfaceRef)

func IOSurfaceRemoveValue(IOSurfaceRef, CFString)

Deletes a value in the dictionary associated with the buffer.

func IOSurfaceSetOwnershipIdentity(IOSurfaceRef, task_id_token_t, Int32, UInt32) -> kern_return_t

func IOSurfaceSetPurgeable(IOSurfaceRef, UInt32, UnsafeMutablePointer&lt;UInt32>?) -> kern_return_t

func IOSurfaceSetValue(IOSurfaceRef, CFString, CFTypeRef)

Sets a value in the dictionary associated with the buffer.

func IOSurfaceSetValues(IOSurfaceRef, CFDictionary)

func IOSurfaceUnlock(IOSurfaceRef, IOSurfaceLockOptions, UnsafeMutablePointer&lt;UInt32>?) -> kern_return_t

“Unlock” an IOSurface for reading or writing.

## See Also

### Reference

IOSurface Structures

IOSurface Constants

