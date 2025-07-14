

- Core Media
-  CMBlockBufferFillDataBytes(with:blockBuffer:offsetIntoDestination:dataLength:) 

Function

# CMBlockBufferFillDataBytes(with:blockBuffer:offsetIntoDestination:dataLength:)

Fills the destination buffer with the specified data byte.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferFillDataBytes(
    with fillByte: CChar,
    blockBuffer destinationBuffer: CMBlockBuffer,
    offsetIntoDestination: Int,
    dataLength: Int
) -> OSStatus
```

## Parameters 

`fillByte`  

The data byte with which to fill the destination buffer.

`destinationBuffer`  

`CMBlockBuffer` into which the data bytes are filled.

`offsetIntoDestination`  

Start of data area for the buffer.

`dataLength`  

Length of the valid data area for the buffer.

## Return Value

Returns `kCMBlockBufferNoErr` if successful.

## See Also

### Modifying a Block Buffer

func CMBlockBufferAppendMemoryBlock(CMBlockBuffer, memoryBlock: UnsafeMutableRawPointer?, length: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a memory block to an existing block buffer.

func CMBlockBufferAppendBufferReference(CMBlockBuffer, targetBBuf: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a reference to an existing block buffer.

func CMBlockBufferAssureBlockMemory(CMBlockBuffer) -> OSStatus

Assures that the system allocates memory for all memory blocks in a block buffer.

func CMBlockBufferAccessDataBytes(CMBlockBuffer, atOffset: Int, length: Int, temporaryBlock: UnsafeMutableRawPointer, returnedPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Accesses potentially noncontiguous data in a block buffer.

func CMBlockBufferCopyDataBytes(CMBlockBuffer, atOffset: Int, dataLength: Int, destination: UnsafeMutableRawPointer) -> OSStatus

Copies bytes from a block buffer into a provided memory area.

func CMBlockBufferReplaceDataBytes(with: UnsafeRawPointer, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Copies bytes from a given memory block into a block buffer replacing bytes in the underlying data blocks.

