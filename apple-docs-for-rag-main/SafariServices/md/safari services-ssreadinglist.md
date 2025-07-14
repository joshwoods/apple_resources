

- Safari Services
-  SSReadingList 

Class

# SSReadingList

An object for adding items to a user’s Safari Reading List.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class SSReadingList
```

## Topics

### Getting the Reading List Singleton Object

class func `default`() -> SSReadingList?

Returns the Safari Reading List singleton object.

### Checking Whether a URL is Supported by Reading List

class func supportsURL(URL) -> Bool

Determines whether a URL can be added to the Reading List.

### Adding an Item to the Reading List

func addItem(with: URL, title: String?, previewText: String?) throws

Adds an item to the Reading List.

### Constants

Reading List Error Domain

The domain used for Reading List errors.

enum Code

Messages that describe a Safari Reading List error.

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

### Safari Reading List

let SSReadingListErrorDomain: String

The domain for Safari Reading List errors.

enum Code

Messages that describe a Safari Reading List error.

struct SSReadingListError

A Safari Reading List error.

