

- Foundation
-  NSUnarchiver Deprecated

Class

# NSUnarchiver

A decoder that restores data from an archive.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class NSUnarchiver
```

Deprecated

Use NSKeyedUnarchiver instead

## Overview

NSUnarchiver, a concrete subclass of NSCoder, defines methods for decoding a set of Objective-C objects from an archive. Such archives are produced by objects of the NSArchiver class.

In macOS 10.2 and later, NSArchiver and NSUnarchiver have been replaced by NSKeyedArchiver and NSKeyedUnarchiver respectively—see Archives and Serializations Programming Guide.

## Topics

### Initializing an NSUnarchiver

init?(forReadingWith: Data)

Returns an `NSUnarchiver` object initialized to read an archive from a given data object.

### Decoding objects

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object archived in a given `NSData` object.

class func unarchiveObject(withFile: String) -> Any?

Decodes and returns the object archived in the file `path`.

### Managing an NSUnarchiver

var isAtEnd: Bool

A Boolean value that indicates whether the receiver has reached the end of the encoded data while decoding.

var systemVersion: UInt32

The system version number in effect when the archive was created.

### Substituting classes or objects

class func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class used when instantiating objects whose ostensible class, according to the archived data, is a given name.

class func decodeClassName(String, asClassName: String)

Instructs instances of `NSUnarchiver` to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class that will be used when instantiating objects whose ostensible class, according to the archived data, is a given name.

func decodeClassName(String, asClassName: String)

Instructs the receiver to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

func replace(Any, with: Any)

Causes the receiver to substitute one given object for another whenever the latter is extracted from the archive.

## Relationships

### Inherits From

- NSCoder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Deprecated

class NSArchiver

A coder that stores an object’s data to an archive.

Deprecated

