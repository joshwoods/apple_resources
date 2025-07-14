

- Foundation
-  NSData 

Class

# NSData

A static byte buffer in memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSData
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

In Swift, the buffer bridges to Data; use NSData when you need reference semantics or other Foundation-specific behavior.

NSData and its mutable subclass NSMutableData provide data objects, or object-oriented wrappers for byte buffers. Data objects let simple allocated buffers (that is, data with no embedded pointers) take on the behavior of Foundation objects.

The size of the data is subject to a theoretical limit of about 8 exabytes (1 EB = 10¹⁸ bytes; in practice, the limit should not be a factor).

NSData is *toll-free bridged* with its Core Foundation counterpart, CFData. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the Data structure, which bridges to the NSData class and its mutable subclass NSMutableData. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

### Writing Data Atomically

NSData provides methods for atomically saving their contents to a file, which guarantee that the data is either saved in its entirety, or it fails completely. An atomic write first writes the data to a temporary file and then, only if this write succeeds, moves the temporary file to its final location.

Although atomic write operations minimize the risk of data loss due to corrupt or partially written files, they may not be appropriate when writing to a temporary directory, the user’s home directory or other publicly accessible directories. When you work with a publicly accessible file, treat that file as an untrusted and potentially dangerous resource. An attacker may compromise or corrupt these files. The attacker can also replace the files with hard or symbolic links, causing your write operations to overwrite or corrupt other system resources.

Avoid using the write(to:atomically:) method (and the related methods) when working inside a publicly accessible directory. Instead, use FileHandle with an existing file descriptor to securely write the file.

For more information, see Securing File Operations in Secure Coding Guide.

## Topics

### Creating Data

init(bytes: UnsafeRawPointer?, length: Int)

Initializes a data object filled with a given number of bytes copied from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Initializes a data object filled with a given number of bytes of data from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?)

Initializes a data object filled with a given number of bytes of data from a given buffer, with a custom deallocator block.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, freeWhenDone: Bool)

Initializes a newly allocated data object by adding the given number of bytes from the given buffer.

init(data: Data)

Initializes a data object with the contents of another data object.

### Reading Data from a File

convenience init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL.

convenience init(contentsOfURL: URL, options: NSData.ReadingOptions) throws

Creates a data object from the data at the provided file URL using specific reading options.

init?(contentsOfFile: String)

Initializes a data object with the content of the file at a given path.

init(contentsOfFile: String, options: NSData.ReadingOptions) throws

Initializes a data object with the content of the file at a given path.

init?(contentsOfURL: URL)

Creates a data object from the data at the specified file URL, or returns `nil` if the system can’t create one.

init(contentsOfURL: URL, options: NSData.ReadingOptions) throws

Creates a data object from the data at the provided file URL using specific reading options.

struct ReadingOptions

Options for methods used to read data objects.

init?(contentsOfMappedFile: String)

Initializes a data object with the contents of the mapped file specified by a given path.

Deprecated

class func dataWithContentsOfMappedFile(String) -> Any?

Creates a data object from the mapped file at a given path.

Deprecated

### Writing Data to a File

func write(toFile: String, atomically: Bool) -> Bool

Writes the data object’s bytes to the file specified by a given path.

func write(toFile: String, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the file specified by a given path.

func write(to: URL, atomically: Bool) -> Bool

Writes the data object’s bytes to the location specified by a given URL.

func write(to: URL, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the location specified by a given URL.

struct WritingOptions

Options for methods used to write data objects.

### Encoding and Decoding Base64 Representations

init?(base64EncodedData: Data, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded data.

init?(base64Encoding: String)

Initializes a data object initialized with the given Base64 encoded string.

Deprecated

init?(base64EncodedString: String, options: NSData.Base64DecodingOptions)

Initializes a data object with the given Base64 encoded string.

func base64EncodedData(options: NSData.Base64EncodingOptions) -> Data

Creates a Base64, UTF-8 encoded data object from the string using the given options.

func base64EncodedString(options: NSData.Base64EncodingOptions) -> String

Creates a Base64 encoded string from the string using the given options.

func base64Encoding() -> String

Initializes a Base64 encoded string from the string.

Deprecated

struct Base64EncodingOptions

Options for methods used to Base64 encode data.

struct Base64DecodingOptions

Options to modify the decoding algorithm used to decode Base64 encoded data.

### Accessing Underlying Bytes

var bytes: UnsafeRawPointer

A pointer to the data object’s contents.

func enumerateBytes((UnsafeRawPointer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates each range of bytes in the data object using a block.

func getBytes(UnsafeMutableRawPointer)

Copies a data object’s contents into a given buffer.

Deprecated

func getBytes(UnsafeMutableRawPointer, length: Int)

Copies a number of bytes from the start of the data object into a given buffer.

func getBytes(UnsafeMutableRawPointer, range: NSRange)

Copies a range of bytes from the data object into a given buffer.

### Finding Data

func subdata(with: NSRange) -> Data

Returns a new data object containing the data object’s bytes that fall within the limits specified by a given range.

func range(of: Data, options: NSData.SearchOptions, in: NSRange) -> NSRange

Finds and returns the range of the first occurrence of the given data, within the given range, subject to given options.

struct SearchOptions

Options for method used to search data objects.

### Testing Data

func isEqual(to: Data) -> Bool

Returns a Boolean value indicating whether this data object is the same as another.

var length: Int

The number of bytes contained by the data object.

### Describing Data

var description: String

### Compressing and Decompressing Data

func compressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by compressing the data object’s bytes.

func decompressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by decompressing data object’s bytes.

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

- NSObject

### Inherited By

- NSMutableData

### Conforms To

- BidirectionalCollection
- CKRecordValue
- CKRecordValueProtocol
- CVarArg
- Collection
- Copyable
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

