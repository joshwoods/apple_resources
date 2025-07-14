

- Core Media
-  CMBlockBufferAssureBlockMemory(\_:) 

Function

# CMBlockBufferAssureBlockMemory(\_:)

Assures that the system allocates memory for all memory blocks in a block buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferAssureBlockMemory(_ theBuffer: CMBlockBuffer) -> OSStatus
```

## Parameters 

`theBuffer`  

`CMBlockBuffer` to operate on. Must not be `NULL`.

## Return Value

Returns `kCMBlockBufferNoErr` if successful.

## Discussion

Traverses the possibly complex `CMBlockBuffer`, allocating the memory for any constituent memory blocks that are not yet allocated.

## See Also

### Modifying a Block Buffer

func CMBlockBufferAppendMemoryBlock(CMBlockBuffer, memoryBlock: UnsafeMutableRawPointer?, length: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a memory block to an existing block buffer.

func CMBlockBufferAppendBufferReference(CMBlockBuffer, targetBBuf: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a reference to an existing block buffer.

func CMBlockBufferAccessDataBytes(CMBlockBuffer, atOffset: Int, length: Int, temporaryBlock: UnsafeMutableRawPointer, returnedPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Accesses potentially noncontiguous data in a block buffer.

func CMBlockBufferCopyDataBytes(CMBlockBuffer, atOffset: Int, dataLength: Int, destination: UnsafeMutableRawPointer) -> OSStatus

Copies bytes from a block buffer into a provided memory area.

func CMBlockBufferReplaceDataBytes(with: UnsafeRawPointer, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Copies bytes from a given memory block into a block buffer replacing bytes in the underlying data blocks.

func CMBlockBufferFillDataBytes(with: CChar, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Fills the destination buffer with the specified data byte.

