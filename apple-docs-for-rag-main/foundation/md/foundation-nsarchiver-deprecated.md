

- Foundation
-  NSArchiver Deprecated

Class

# NSArchiver

A coder that stores an object’s data to an archive.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class NSArchiver
```

Deprecated

Use NSKeyedArchiver instead

## Overview

NSArchiver, a concrete subclass of NSCoder, provides a way to encode objects into an architecture-independent format that can be stored in a file. When you archive a graph of objects, the class information and instance variables for each object are written to the archive. The companion class NSUnarchiver decodes the data in an archive and creates a graph of objects equivalent to the original set.

NSArchiver stores the archive data in a mutable data object (NSMutableData). After encoding the objects, you can have the NSArchiver object write this mutable data object immediately to a file, or you can retrieve the mutable data object for some other use.

In macOS 10.2 and later, NSArchiver and NSUnarchiver have been replaced by NSKeyedArchiver and NSKeyedUnarchiver respectively—see Archives and Serializations Programming Guide.

## Topics

### Initializing an NSArchiver

init(forWritingWith: NSMutableData)

Returns an archiver, initialized to encode stream and version information into a given mutable data object.

### Archiving data

class func archivedData(withRootObject: Any) -> Data

Returns a data object containing the encoded form of the object graph whose root object is given.

class func archiveRootObject(Any, toFile: String) -> Bool

Creates a temporary instance of `NSArchiver` and archives an object graph by encoding it into a data object and writing the resulting data object to a specified file.

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

func encodeConditionalObject(Any?)

Conditionally archives a given object.

### Getting the archived data

var archiverData: NSMutableData

The receiver’s archive data.

### Substituting classes or objects

func classNameEncoded(forTrueClassName: String) -> String?

Returns the name of the class used to archive instances of the class with a given true name.

func encodeClassName(String, intoClassName: String)

Encodes a substitute name for the class with a given true name.

func replace(Any, with: Any)

Causes the receiver to treat subsequent requests to encode a given object as though they were requests to encode another given object.

### Constants

Archiving Exception Names

Raised by `NSArchiver` if there are problems initializing or encoding.

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

class NSUnarchiver

A decoder that restores data from an archive.

Deprecated

