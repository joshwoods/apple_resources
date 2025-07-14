

- Foundation
-  NSURLQueryItem 

Class

# NSURLQueryItem

An object representing a single name/value pair for an item in the query portion of a URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSURLQueryItem
```

## Overview

In Swift, this object bridges to URLQueryItem; use NSURLQueryItem when you need reference semantics or other Foundation-specific behavior.

You use query items with the queryItems property of an NSURLComponents object.

Important

The Swift overlay to the Foundation framework provides the URLQueryItem structure, which bridges to the NSURLQueryItem class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating a Query Item

init(name: String, value: String?)

Initializes a newly allocated query item with the specified name and value.

### Reading a Query Item’s Name and Value

var name: String

The name of the query item.

var value: String?

The value for the query item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

