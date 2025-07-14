

- Foundation
-  URLQueryItem 

Structure

# URLQueryItem

A single name-value pair from the query portion of a URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLQueryItem
```

## Topics

### Creating Query Items

init(name: String, value: String?)

Creates a new query item with the name and value you specify.

### Accessing the Item’s Components

var name: String

The name of the query item.

var value: String?

The value for the query item.

### Using Reference Types

class NSURLQueryItem

An object representing a single name/value pair for an item in the query portion of a URL.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### URLs

struct URL

A value that identifies the location of a resource, such as an item on a remote server or the path to a local file.

struct URLComponents

A structure that parses URLs into and constructs URLs from their constituent parts.

