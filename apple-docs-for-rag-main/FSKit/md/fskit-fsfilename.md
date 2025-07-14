

- FSKit
-  FSFileName 

Class

# FSFileName

The name of a file, expressed as a data buffer.

macOS 15.4+

``` source
class FSFileName
```

## Overview

`FSFileName` is the class that carries filenames from the kernel to `FSModule` instances, and carries names back to the kernel as part of directory enumeration.

A filename is usually a valid UTF-8 sequence, but can be an arbitrary byte sequence that doesn’t conform to that format. As a result, the data property always contains a value, but the string property may be empty. An `FSModule` can receive an `FSFileName` that isn’t valid UTF-8 in two cases:

1.  A program passes erroneous data to a system call. The `FSModule` treats this situation as an error.

2.  An `FSModule` lacks the character encoding used for a file name. This situation occurs because some file system formats consider a filename to be an arbitrary “bag of bytes,” and leave character encoding up to the operating system. Without encoding information, the `FSModule` can only pass back the names it finds on disk. In this case, the behavior of upper layers such as NSFileManager is unspecified. However, the `FSModule` must support looking up such names and using them as the source name of rename operations. The `FSModule` must also be able to support filenames that are derivatives of filenames returned from directory enumeration. Derivative filenames include Apple Double filenames (`"._Name"`), and editor backup filenames.

Important

Don’t subclass this class.

## Topics

### Creating a filename

convenience init(bytes: UnsafeBufferPointer&lt;CChar>)

convenience init(cString: UnsafeBufferPointer&lt;CChar>)

convenience init(data: Data)

Creates a filename by copying a character sequence data object.

convenience init(string: String)

Creates a filename by copying a character sequence from a string instance.

### Accessing filename properties

var data: Data

The byte sequence of the filename, as a data object.

var string: String?

The filename, represented as a Unicode string.

var debugDescription: String

The filename, represented as a potentially lossy conversion to a string.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### File systems

class FSUnaryFileSystem

An abstract base class for implementing a minimal file system.

protocol FSFileSystemBase

A protocol containing functionality supplied by FSKit to file system implementations.

