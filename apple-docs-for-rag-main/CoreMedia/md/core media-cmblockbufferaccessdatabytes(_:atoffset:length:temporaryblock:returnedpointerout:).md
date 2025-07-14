

- Core Media
-  CMBlockBufferAccessDataBytes(\_:atOffset:length:temporaryBlock:returnedPointerOut:) 

Function

# CMBlockBufferAccessDataBytes(\_:atOffset:length:temporaryBlock:returnedPointerOut:)

Accesses potentially noncontiguous data in a block buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferAccessDataBytes(
    _ theBuffer: CMBlockBuffer,
    atOffset offset: Int,
    length: Int,
    temporaryBlock: UnsafeMutableRawPointer,
    returnedPointerOut: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`theBuffer`  

`CMBlockBuffer` to operate on. Must not be `NULL`.

`offset`  

Offset within the `CMBlockBuffer's` offset range.

`length`  

Desired number of bytes to access at offset.

`temporaryBlock`  

A piece of memory, assumed to be at least `length` bytes in size. Must not be `NULL`

`returnedPointerOut`  

Receives `NULL` if the desired amount of data could not be accessed at the given offset. Receives non-`NULL` if it could. The value returned is either a direct pointer into the `CMBlockBuffer` or to the `temporaryBlock`. Must not be `NULL`.

## Return Value

Returns `kCMBlockBufferNoErr` if the desired amount of data could be accessed at the given offset.

## Discussion

This routine is use for accessing contiguous and noncontiguous data. If the data is contiguous, the routine will return a pointer to the given `CMBlockBuffer`. If the data is not contiguous, the routine will copy the data into a temporary block and a pointer to this block will be returned.

## See Also

### Modifying a Block Buffer

func CMBlockBufferAppendMemoryBlock(CMBlockBuffer, memoryBlock: UnsafeMutableRawPointer?, length: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a memory block to an existing block buffer.

func CMBlockBufferAppendBufferReference(CMBlockBuffer, targetBBuf: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a reference to an existing block buffer.

func CMBlockBufferAssureBlockMemory(CMBlockBuffer) -> OSStatus

Assures that the system allocates memory for all memory blocks in a block buffer.

func CMBlockBufferCopyDataBytes(CMBlockBuffer, atOffset: Int, dataLength: Int, destination: UnsafeMutableRawPointer) -> OSStatus

Copies bytes from a block buffer into a provided memory area.

func CMBlockBufferReplaceDataBytes(with: UnsafeRawPointer, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Copies bytes from a given memory block into a block buffer replacing bytes in the underlying data blocks.

func CMBlockBufferFillDataBytes(with: CChar, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Fills the destination buffer with the specified data byte.

