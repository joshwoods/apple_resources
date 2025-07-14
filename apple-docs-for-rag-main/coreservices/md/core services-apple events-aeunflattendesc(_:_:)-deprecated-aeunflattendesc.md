

- Core Services
- Apple Events
-  AEUnflattenDesc(\_:\_:) Deprecated

Function

# AEUnflattenDesc(\_:\_:)

Unflattens the data in the passed buffer and creates a descriptor from it.

macOS 10.0–11.0Deprecated

``` source
func AEUnflattenDesc(
    _ buffer: UnsafeRawPointer!,
    _ result: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`buffer`  

A pointer to memory, allocated by the application, that contains flattened data produced by a previous call to AEFlattenDesc(_:_:_:_:).

`result`  

A null descriptor. On successful completion, points to a descriptor created from the flattened data. The caller is responsible for disposing of the descriptor.

## Return Value

A result code. Returns `paramErr` if the flattened data in `buffer` is found to be invalid. See Result Codes for other possible values.

## Discussion

This function assumes the passed buffer contains valid flattened data, produced by a previous call to AEFlattenDesc(_:_:_:_:). See that function for a description of when you might want to flatten and unflatten descriptors, and of possible limitations.

Flattening and unflattening works across OS versions, including between Mac OS 9 and macOS.

Flattening is endian-neutral. That is, you can save flattened data on a machine that is either big-endian or little-endian, then retrieve and unflatten the data on either type of machine, without any special steps by your application.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Serializing Apple Event Data

func AESizeOfFlattenedDesc(UnsafePointer&lt;AEDesc>!) -> Size

Returns the amount of buffer space needed to store the descriptor after flattening it.

func AEFlattenDesc(UnsafePointer&lt;AEDesc>!, Ptr!, Size, UnsafeMutablePointer&lt;Size>!) -> OSStatus

Flattens the specified descriptor and stores the data in the supplied buffer.

