

- AVFoundation
-  AVMediaDataStorage 

Class

# AVMediaDataStorage

An object that represents the media sample data storage file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
class AVMediaDataStorage
```

## Topics

### Creating Media Data Storage

init(url: URL, options: [String : Any]?)

Creates a media data storage object associated with a file URL.

### Accessing the URL

func url() -> URL?

Returns the URL used to initialize the receiver.

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

