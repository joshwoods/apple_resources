

- Foundation
-  NSUUID 

Class

# NSUUID

A universally unique value that can be used to identify types, interfaces, and other items.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSUUID
```

## Overview

In Swift, this object bridges to UUID; use NSUUID when you need reference semantics or other Foundation-specific behavior.

UUIDs (Universally Unique Identifiers), also known as GUIDs (Globally Unique Identifiers) or IIDs (Interface Identifiers), are 128-bit values. UUIDs created by `NSUUID` conform to RFC 4122 version 4 and are created with random bytes.

The standard format for UUIDs represented in ASCII is a string punctuated by hyphens, for example `68753A44-4D6F-1226-9C60-0050E4C00067`. The hex representation looks, as you might expect, like a list of numerical values preceded by 0x. For example, `0xD7`, `0x36`, `0x95`, `0x0A`, `0x4D`, `0x6E`, `0x12`, `0x26`, `0x80`, `0x3A`, `0x00`, `0x50`, `0xE4`, `0xC0`, `0x00`, `0x67`. Because a UUID is expressed simply as an array of bytes, there are no endianness considerations for different platforms.

The `NSUUID` class is *not* toll-free bridged with CoreFoundation’s CFUUID. Use UUID strings to convert between `CFUUIDRef` and `NSUUID`, if needed. Two `NSUUID` objects are not guaranteed to be comparable by pointer value (as CFUUID is); use isEqual(_:) to compare two `NSUUID` instances.

Important

The Swift overlay to the Foundation framework provides the UUID structure, which bridges to the NSUUID class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating UUIDs

init()

Initializes a new UUID with RFC 4122 version 4 random bytes.

convenience init?(uuidString: String)

Initializes a new UUID with the formatted string.

convenience init(uuidBytes: UnsafePointer&lt;UInt8>?)

Initializes a new UUID with the given bytes.

### Get UUID Values

func getBytes(UnsafeMutablePointer&lt;UInt8>)

Returns the UUID as bytes.

var uuidString: String

The UUID as a string.

### Instance Methods

func compare(UUID) -> ComparisonResult

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

