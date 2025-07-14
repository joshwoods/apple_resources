

- Background Assets
-  BADownload 

Class

# BADownload

An object that represents an in-progress or concluded asset download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
class BADownload
```

## Overview

Note

You don’t create instances of this object directly. Instead, use an object that inherits from BADownload, such as BAURLDownload.

## Topics

### Getting the identity

var identifier: String

The app-specific string that uniquely identifies the downloadable asset.

var uniqueIdentifier: String

The system-provided string that uniquely identifies the download object.

### Determining the priority

var isEssential: Bool

var priority: BADownload.Priority

The download’s execution priority.

struct Priority

A type that determines the execution priority of a scheduled asset download.

### Getting the current state

var state: BADownload.State

The current state of the download.

enum State

Constants that indicate the state of a download.

### Downloading nonessential assets

func removingEssential() -> Self

## Relationships

### Inherits From

- NSObject

### Inherited By

- BAURLDownload

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
- Sendable

## See Also

### Asset downloads

class BAURLDownload

An object that represents a remote asset to download.

struct Priority

A type that determines the execution priority of a scheduled asset download.

