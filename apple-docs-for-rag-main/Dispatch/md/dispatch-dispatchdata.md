

- Dispatch
-  DispatchData 

Structure

# DispatchData

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DispatchData
```

## Overview

The memory buffer managed by this object may be a single contiguous block of memory, or it may consist of multiple discontiguous blocks. For the discontiguous case, the dispatch data object makes it appear as if the memory is contiguous.

## Topics

### Creating a Dispatch Data Structure

init(bytes: UnsafeRawBufferPointer)

Creates a new dispatch data object from the specified memory buffer.

init(bytesNoCopy: UnsafeRawBufferPointer, deallocator: DispatchData.Deallocator)

Creates a new dispatch data object using the specified memory buffer and deallocator.

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

enum Deallocator

Memory deallocators for dispatch data objects.

static let empty: DispatchData

A dispatch data object representing a zero-length memory region.

### Appending Data to the Buffer

func append(DispatchData)

func append&lt;SourceType>(UnsafeBufferPointer&lt;SourceType>)

func append(UnsafeRawBufferPointer)

### Copying Bytes

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int)

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;DispatchData.Index>?) -> Int

func copyBytes(to: UnsafeMutableRawBufferPointer, from: Range&lt;DispatchData.Index>)

### Accessing Buffer Data

subscript(DispatchData.Index) -> UInt8

func region(location: Int) -> (data: DispatchData, offset: Int)

struct Region

### Iterating Over the Buffer Contents

func makeIterator() -> DispatchData.Iterator

func enumerateBytes((UnsafeBufferPointer&lt;UInt8>, Int, inout Bool) -> Void)

### Retrieving Buffer Subsequences

func subdata(in: Range&lt;DispatchData.Index>) -> DispatchData

### Combining Sequence Elements

func append(DispatchData)

func append&lt;SourceType>(UnsafeBufferPointer&lt;SourceType>)

func append(UnsafeRawBufferPointer)

func append(UnsafePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int)

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;DispatchData.Index>?) -> Int

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;DispatchData.Index>)

func copyBytes(to: UnsafeMutableRawBufferPointer, from: Range&lt;DispatchData.Index>)

func enumerateBytes((UnsafeBufferPointer&lt;UInt8>, Int, inout Bool) -> Void)

func makeIterator() -> DispatchData.Iterator

func region(location: Int) -> (data: DispatchData, offset: Int)

func subdata(in: Range&lt;DispatchData.Index>) -> DispatchData

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

### Deprecated

init(bytes: UnsafeBufferPointer&lt;UInt8>)

Initialize a data object with copied memory content.

init(bytesNoCopy: UnsafeBufferPointer&lt;UInt8>, deallocator: DispatchData.Deallocator)

Initialize a data object without copying the bytes.

func append(UnsafePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;DispatchData.Index>)

### Instance Methods

func enumerateBytes(block: (UnsafeBufferPointer&lt;UInt8>, Int, inout Bool) -> Void)

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- DataProtocol
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### System Event Monitoring

class DispatchSource

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

Dispatch Source

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

class DispatchIO

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

struct DispatchDataIterator

A byte-by-byte iterator over the contents of a dispatch data object.

Dispatch I/O

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

Dispatch Data

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

protocol DispatchSourceProtocol

Defines a common set of properties and methods that are shared with all dispatch source types.

