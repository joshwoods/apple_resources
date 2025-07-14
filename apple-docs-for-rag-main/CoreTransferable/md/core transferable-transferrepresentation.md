

- Core Transferable
-  TransferRepresentation 

Protocol

# TransferRepresentation

A declarative description of the process of importing and exporting a transferable item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol TransferRepresentation : Sendable
```

## Overview

Combine multiple existing transfer representations to compose a single transfer representation that describes how to transfer an item in multiple scenarios.

The following shows a `Greeting` type that transfers both as a `Codable` type and by proxy through its `message` string.

```
import UniformTypeIdentifiers

struct Greeting: Codable, Transferable {
    let message: String
    var displayInAllCaps: Bool = false

    static var transferRepresentation: some TransferRepresentation {
        CodableRepresentation(contentType: .greeting)
        ProxyRepresentation(exporting: \.message)
    }
}

extension UTType {
    static var greeting: UTType { .init(exportedAs: "com.example.greeting") }
}
```

## Topics

### Implementing a transfer representation

var body: Self.Body

A builder expression that describes the process of importing and exporting an item.

**Required**

associatedtype Body : TransferRepresentation

The transfer representation for the item.

**Required**

associatedtype Item : Transferable

The type of the item that’s being transferred.

**Required**

### Configuring exports

func exportingCondition((Self.Item) -> Bool) -> _ConditionalTransferRepresentation&lt;Self>

Prevents the system from exporting an item if it does not meet the supplied condition.

### Controlling visibility

func visibility(TransferRepresentationVisibility) -> some TransferRepresentation&lt;Self.Item> 

Specifies the kinds of apps and processes that can see an item in transit.

### Instance Methods

func suggestedFileName(String) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

func suggestedFileName((Self.Item) -> String?) -> some TransferRepresentation&lt;Self.Item> 

Provides a filename to use if the receiver chooses to write the item to disk.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- CodableRepresentation
- DataRepresentation
- FileRepresentation
- ProxyRepresentation
- TupleTransferRepresentation

## See Also

### Essentials

protocol Transferable

A protocol that describes how a type interacts with transport APIs such as drag and drop or copy and paste.

Choosing a transfer representation for a model type

Define a custom representation for your data using a combination of built-in types.

