

- Foundation
-  NSMutableData 

Class

# NSMutableData

An object representing a dynamic byte buffer in memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableData
```

## Overview

In Swift, this object bridges to Data; use NSMutableData when you need reference semantics or other Foundation-specific behavior.

`NSMutableData` and its superclass `NSData` provide data objects, or object-oriented wrappers for byte buffers. Data objects let simple allocated buffers (that is, data with no embedded pointers) take on the behavior of Foundation objects. They are typically used for data storage and are also useful in Distributed Objects applications, where data contained in data objects can be copied or moved between applications. `NSData` creates static data objects, and `NSMutableData` creates dynamic data objects. You can easily convert one type of data object to the other with the initializer that takes an `NSData` object or an `NSMutableData` object as an argument.

The following NSData methods change when used on a mutable data object:

- init(bytesNoCopy:length:freeWhenDone:)

- init(bytesNoCopy:length:deallocator:)

- init(bytesNoCopy:length:)

- dataWithBytesNoCopy:length:freeWhenDone:

- dataWithBytesNoCopy:length:

When called, the bytes are immediately copied and then the buffer is freed.

`NSMutableData` is “toll-free bridged” with its Core Foundation counterpart, CFData. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the Data structure, which bridges to the NSMutableData class and its immutable superclass NSData. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating Mutable Data

init?(capacity: Int)

Returns an initialized mutable data object capable of holding the specified number of bytes.

init?(length: Int)

Initializes and returns a mutable data object containing a given number of zeroed bytes.

### Accessing Raw Bytes

var mutableBytes: UnsafeMutableRawPointer

A pointer to the data contained by the mutable data object.

### Counting Bytes

var length: Int

The number of bytes contained in the mutable data object.

### Adding Bytes

func append(UnsafeRawPointer, length: Int)

Appends to the receiver a given number of bytes from a given buffer.

func append(Data)

Appends the content of another data object to the receiver.

func increaseLength(by: Int)

Increases the length of the receiver by a given number of bytes.

### Modifying Bytes

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer)

Replaces with a given set of bytes a given range within the contents of the receiver.

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer?, length: Int)

Replaces with a given set of bytes a given range within the contents of the receiver.

func resetBytes(in: NSRange)

Replaces with zeroes the contents of the receiver in a given range.

func setData(Data)

Replaces the entire contents of the receiver with the contents of another data object.

### Compressing and Decompressing Data

func compress(using: NSData.CompressionAlgorithm) throws

Compresses the data object’s bytes using an algorithm that you specify.

func decompress(using: NSData.CompressionAlgorithm) throws

Decompresses the data object’s bytes.

enum CompressionAlgorithm

An algorithm that indicates how to compress or decompress data.

var NSCompressionErrorMaximum: Int

The end of the range of error codes reserved for compression errors.

var NSCompressionErrorMinimum: Int

The start of the range of error codes reserved for compression errors.

var NSCompressionFailedError: Int

An error code value that indicates a failure to compress data using the provided algorithm.

var NSDecompressionFailedError: Int

An error code value that indicates a failure to decompress data using the provided algorithm.

## Relationships

### Inherits From

- NSData

### Inherited By

- NSPurgeableData

### Conforms To

- BidirectionalCollection
- CVarArg
- Collection
- CustomDebugStringConvertible
- CustomStringConvertible
- DataProtocol
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- RandomAccessCollection
- Sequence

