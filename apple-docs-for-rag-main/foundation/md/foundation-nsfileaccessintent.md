

- Foundation
-  NSFileAccessIntent 

Class

# NSFileAccessIntent

The details of a coordinated-read or coordinated-write operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSFileAccessIntent
```

## Overview

Use this class when performing asynchronous operations with a file coordinator using the coordinator’s coordinate(with:queue:byAccessor:) method.

## Topics

### Creating a File Access Intent

class func readingIntent(with: URL, options: NSFileCoordinator.ReadingOptions) -> Self

Returns a file access intent object for reading the given URL with the provided options.

class func writingIntent(with: URL, options: NSFileCoordinator.WritingOptions) -> Self

Returns a file access intent object for writing to the given URL with the provided options.

### Accessing the Current URL

var url: URL

The current URL for the item managed by the file access intent instance. (read-only)

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

### Coordinated file access

protocol NSFilePresenter

The interface a file coordinator uses to inform an object presenting a file about changes to that file made elsewhere in the system.

class NSFileCoordinator

An object that coordinates the reading and writing of files and directories among file presenters.

