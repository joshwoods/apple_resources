

- Foundation
-  Pipe 

Class

# Pipe

A one-way communications channel between related processes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Pipe
```

## Overview

Pipe objects provide an object-oriented interface for accessing pipes. An Pipe object represents both ends of a pipe and enables communication through the pipe. A pipe is a one-way communications channel between related processes; one process writes data, while the other process reads that data. The data that passes through the pipe is buffered; the size of the buffer is determined by the underlying operating system. Pipe is an abstract class, the public interface of a class cluster.

## Topics

### Getting the File Handles for a Pipe

var fileHandleForReading: FileHandle

The receiver’s read file handle.

var fileHandleForWriting: FileHandle

The receiver’s write file handle.

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
- Sendable

## See Also

### Tasks and Pipes

class Process

An object that represents a subprocess of the current process.

