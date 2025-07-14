

- Foundation
-  NSURLHandle 

Class

# NSURLHandle

An object that accesses and manages resource data indicated by a URL.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSURLHandle
```

## Overview

Important

NSURLHandle is deprecated in macOS 10.4 and later. Use URLSession instead.

A single NSURLHandle can service multiple equivalent NSURL objects, but only if these URLs map to the same resource.

### Overview

Cocoa provides private concrete subclasses to handle HTTP and file URL schemes. If you want to implement support for additional URL schemes, you would do so by creating a subclass of `NSURLHandle`. You can use `NSURL` and `NSURLHandle` to download from FTP sites without subclassing.

## Topics

### Loading resource data

enum Status

These following constants are defined by `NSURLHandle` and are returned by status.

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

