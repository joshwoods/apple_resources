

- FSKit
-  FSUnaryFileSystem 

Class

# FSUnaryFileSystem

An abstract base class for implementing a minimal file system.

macOS 15.4+

``` source
class FSUnaryFileSystem
```

## Overview

`FSUnaryFileSystem` is a simplified file system, which works with one FSResource and presents it as one FSVolume.

The one volume and its container have a shared state and lifetime, a more constrained life cycle than the FSFileSystem design flow.

Implement your app extension by providing a subclass of `FSUnaryFileSystem` as a delegate object. Your delegate also needs to implement the FSUnaryFileSystemOperations protocol so that it can load resources.

## Topics

### Implementing operations

protocol FSUnaryFileSystemOperations

Operations performed by a unary file system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- FSFileSystemBase
- Hashable
- NSObjectProtocol

## See Also

### File systems

protocol FSFileSystemBase

A protocol containing functionality supplied by FSKit to file system implementations.

class FSFileName

The name of a file, expressed as a data buffer.

