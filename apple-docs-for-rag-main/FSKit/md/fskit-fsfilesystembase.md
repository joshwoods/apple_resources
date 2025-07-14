

- FSKit
-  FSFileSystemBase 

Protocol

# FSFileSystemBase

A protocol containing functionality supplied by FSKit to file system implementations.

macOS 15.4+

``` source
protocol FSFileSystemBase : NSObjectProtocol
```

## Overview

Both FSFileSystem and FSUnaryFileSystem conform to this protocol.

## Topics

### Instance Properties

var containerStatus: FSContainerStatus

The status of the file system container, indicating its readiness and activity.

**Required**

### Instance Methods

func wipe(FSBlockDeviceResource, completionHandler: ((any Error)?) -> Void)

Wipes existing file systems on the specified resource.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- FSUnaryFileSystem

## See Also

### File systems

class FSUnaryFileSystem

An abstract base class for implementing a minimal file system.

class FSFileName

The name of a file, expressed as a data buffer.

