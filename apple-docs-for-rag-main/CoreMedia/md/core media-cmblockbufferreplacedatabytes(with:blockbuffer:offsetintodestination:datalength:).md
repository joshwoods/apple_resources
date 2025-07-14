

- Core Media
-  CMBlockBufferReplaceDataBytes(with:blockBuffer:offsetIntoDestination:dataLength:) 

Function

# CMBlockBufferReplaceDataBytes(with:blockBuffer:offsetIntoDestination:dataLength:)

Copies bytes from a given memory block into a block buffer replacing bytes in the underlying data blocks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferReplaceDataBytes(
    with sourceBytes: UnsafeRawPointer,
    blockBuffer destinationBuffer: CMBlockBuffer,
    offsetIntoDestination: Int,
    dataLength: Int
) -> OSStatus
```

## Parameters 

`sourceBytes`  

Memory block from which bytes are copied into the destination `CMBlockBuffer`.

`destinationBuffer`  

`CMBlockBuffer` whose range of bytes will be replaced by the `sourceBytes`.

`offsetIntoDestination`  

Offset within the destination `CMBlockBuffer` at which replacement should begin.

`dataLength`  

Number of bytes to be replaced, starting at `offsetIntoDestination`, in the `destinationBuffer`.

## Return Value

Returns `kCMBlockBufferNoErr` if the replacement succeeded, returns an error otherwise.

## Discussion

This function is used to replace bytes in a `CMBlockBuffer's` memory blocks with those from a provided piece of memory. It deals with the possibility of the destination range of data being noncontiguous. `CMBlockBufferAssureBlockMemory`() is called on the given `CMBlockBuffer`. If desired range is subsequently not accessible in the `CMBlockBuffer`, an error is returned and the contents of the `CMBlockBuffer` are untouched.

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

func CMBlockBufferFillDataBytes(with: CChar, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Fills the destination buffer with the specified data byte.

