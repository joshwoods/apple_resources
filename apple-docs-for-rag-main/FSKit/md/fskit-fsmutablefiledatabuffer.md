

- FSKit
-  FSMutableFileDataBuffer 

Class

# FSMutableFileDataBuffer

A wrapper object for a data buffer.

macOS 15.4+

``` source
class FSMutableFileDataBuffer
```

## Overview

This object provides a “zero-copy” buffer, for use when reading data from files. By not requiring additional buffer copying, this object reduces the extension’s memory footprint and improves performance. The `FSMutableFileDataBuffer` behaves similarly to a `uio` in the kernel.

## Topics

### Accessing buffer properties

func withUnsafeMutableBytes&lt;R, E>((UnsafeMutableRawBufferPointer) throws(E) -> R) throws(E) -> R

Performs the given closure with an unsafe pointer to the underlying bytes of the data buffer.

var length: Int

The data length of the buffer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Reading and writing

func read(from: FSItem, at: off_t, length: Int, into: FSMutableFileDataBuffer, replyHandler: (Int, (any Error)?) -> Void)

Reads the contents of the given file item.

**Required**

func write(contents: Data, to: FSItem, at: off_t, replyHandler: (Int, (any Error)?) -> Void)

Writes contents to the given file item.

**Required**

