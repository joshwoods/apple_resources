

- FSKit
-  FSUnaryFileSystemOperations 

Protocol

# FSUnaryFileSystemOperations

Operations performed by a unary file system.

macOS 15.4+

``` source
protocol FSUnaryFileSystemOperations : NSObjectProtocol
```

## Overview

Make sure your subclass of FSUnaryFileSystem conforms to this protocol.

## Topics

### Loading and unloading resources

func loadResource(resource: FSResource, options: FSTaskOptions, replyHandler: (FSVolume?, (any Error)?) -> Void)

Requests that the file system load a resource and present it as a volume.

**Required**

func unloadResource(resource: FSResource, options: FSTaskOptions, replyHandler: ((any Error)?) -> Void)

Requests that the file system unload the specified resource.

**Required**

func didFinishLoading()

Notifies you that the system finished loading your file system extension.

### Probing resources

func probeResource(resource: FSResource, replyHandler: (FSProbeResult?, (any Error)?) -> Void)

Requests that the file system probe the specified resource.

**Required**

class FSProbeResult

An object that represents the results of a specific probe.

## Relationships

### Inherits From

- NSObjectProtocol

