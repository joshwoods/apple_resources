

- Foundation
-  NSItemProviderWriting 

Protocol

# NSItemProviderWriting

The protocol for implementing a class to allow an item provider to retrieve data from an instance of the class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol NSItemProviderWriting : NSObjectProtocol
```

## Overview

A source app uses an object that conforms to this protocol to initialize an item provider for a copied or dragged item.

## Topics

### Loading data

func loadData(withTypeIdentifier: String, forItemProviderCompletionHandler: (Data?, (any Error)?) -> Void) -> Progress?

Loads data of a particular type, identified by the given UTI.

**Required**

### Getting the writable type identifiers

static var writableTypeIdentifiersForItemProvider: [String]

An array of UTI strings representing the types of data that can be loaded for an item provider.

**Required**

var writableTypeIdentifiersForItemProvider: [String]

An array of UTI strings representing the types of data that can be loaded for an item provider.

### Getting the representation visibility specification

The representation visibility specifications control which categories of processes can see the item provider.

static func itemProviderVisibilityForRepresentation(withTypeIdentifier: String) -> NSItemProviderRepresentationVisibility

Asks the item provider for the default representation visibility specification for the given UTI.

func itemProviderVisibilityForRepresentation(withTypeIdentifier: String) -> NSItemProviderRepresentationVisibility

Asks the item provider for the representation visibility specification for the given UTI.

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

protocol NSItemProviderReading

The protocol for implementing a class to allow an item provider to create an instance of the class.

enum NSItemProviderRepresentationVisibility

Specifications that control which categories of processes can see an item.

enum ErrorCode

The error codes that describe problems with consuming data from an item provider.

