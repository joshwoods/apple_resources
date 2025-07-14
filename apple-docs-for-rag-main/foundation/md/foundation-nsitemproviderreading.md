

- Foundation
-  NSItemProviderReading 

Protocol

# NSItemProviderReading

The protocol for implementing a class to allow an item provider to create an instance of the class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol NSItemProviderReading : NSObjectProtocol
```

## Overview

A destination app uses an object that conforms to this protocol to consume pasted or dropped items.

## Topics

### Creating an object from a pasted or dropped item

static func object(withItemProviderData: Data, typeIdentifier: String) throws -> Self

Creates a new instance of a class using the given data and UTI string.

**Required**

### Getting the readable type identifiers

static var readableTypeIdentifiersForItemProvider: [String]

An array of UTI strings representing the data types supported by the class.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSAttributedString
- NSMutableString
- NSString
- NSURL
- NSUserActivity

## See Also

### Constants

typealias CompletionHandler

A block that receives the item provider’s data.

typealias LoadHandler

A block that loads the item provider’s data and coerces it to the specified type.

Options Dictionary Key

Keys indicating options to use when generating the item provider’s data.

Keys for Items Accessed in JavaScript Code

Keys in property list items that the system recieves from or sends to JavaScript code.

class let errorDomain: String

The error domain associated with the item provider.

struct NSItemProviderFileOptions

Data-access specifications that declare how to handle items.

protocol NSItemProviderWriting

The protocol for implementing a class to allow an item provider to retrieve data from an instance of the class.

enum NSItemProviderRepresentationVisibility

Specifications that control which categories of processes can see an item.

enum ErrorCode

The error codes that describe problems with consuming data from an item provider.

