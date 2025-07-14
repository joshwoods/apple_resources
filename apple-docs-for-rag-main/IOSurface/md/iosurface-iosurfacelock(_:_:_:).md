

- IOSurface
-  IOSurfaceLock(\_:\_:\_:) 

Function

# IOSurfaceLock(\_:\_:\_:)

“Lock” an IOSurface for reading or writing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
func IOSurfaceLock(
    _ buffer: IOSurfaceRef,
    _ options: IOSurfaceLockOptions,
    _ seed: UnsafeMutablePointer?
) -> kern_return_t
```

## Discussion

The term “lock” is used loosely in this context, and is used along with the “unlock” information to put a bound on CPU access to the raw IOSurface data.

If the seed parameter is non-NULL, IOSurfaceLock(_:_:_:) will store the buffer’s internal modification seed value at the time you made the lock call. You can compare this value to a value returned previously to determine of the contents of the buffer has been changed since the last lock.

In the case of IOSurfaceUnlock(_:_:_:), the seed value returned will be the internal seed value at the time of the unlock. If you locked the buffer for writing, this value will be incremented as the unlock is performed and the new value will be returned.

See `IOSurface lock flags` for more information.

Note

Locking and unlocking an IOSurface is not a particularly cheap operation, so care should be taken to avoid the calls whenever possible. The seed values are particularly useful for keeping a cache of the buffer contents.

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

