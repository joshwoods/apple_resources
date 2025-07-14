

- Core Transferable
-  ProxyRepresentation 

Structure

# ProxyRepresentation

A transfer representation that uses another type’s transfer representation as its own.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ProxyRepresentation where Item : Transferable, ProxyRepresentation : Transferable
```

## Mentioned in 

Choosing a transfer representation for a model type

## Overview

Use this representation to rely on an existing transfer representation that’s suitable for the type. For example, a `Note` type might use the String structure’s built-in Transferable conformance — a plain text representation — so it can be pasted into any text editor:

```
struct Note: Transferable {
    var body: String

    static var transferRepresentation: some TransferRepresentation {
        ProxyRepresentation(\.body)
    }
}
```

`ProxyRepresentation` makes it easy to provide alternative representations for receivers that don’t support the preferred custom format.

```
 struct Todo: Transferable, Codable {
    var text: String
    var isDone = false

    static var transferRepresentation: some TransferRepresentation {
        CodableRepresentation(contentType: .todo)
        ProxyRepresentation(\.text)
    }
}

 extension UTType {
     static var todo: UTType { UTType(exportedAs: "com.example.todo") }
 }
```

Write the order of the representations in the `transferRepresentation` property from more preferred to less preferred. In the previous example, if the receiver knows about the custom `com.example.todo` content type, it will receive that custom content type. Using a `ProxyRepresentation` as the alternative lets people paste the to-do item in any text editor that doesn’t support the `com.example.todo` content type but works with text formats.

`ProxyRepresentation` is a convenience, and its evaluation isn’t supposed to be calculation-heavy. Don’t perform long-running work in `exporting` and `importing` closures. They shouldn’t contain network requests, file operations, or other potentially time-consuming tasks as they can cause delays during operations with `Transferable` items.

Use FileRepresentation or DataRepresentation to read and write files or for other lengthy tasks.

## Topics

### Initializers

init(exporting: (Item) async throws -> ProxyRepresentation)

Creates a transfer representation that’s exported by proxy through another transfer representation.

Deprecated

init(exporting: (Item) throws -> ProxyRepresentation)

Creates a transfer representation that’s exported by proxy through another transfer representation.

init(exporting: (Item) throws -> ProxyRepresentation, importing: (ProxyRepresentation) throws -> Item)

Creates a transfer representation that’s imported and exported by proxy through another transfer representation.

init(exporting: (Item) async throws -> ProxyRepresentation, importing: (ProxyRepresentation) async throws -> Item)

Creates a transfer representation that’s imported and exported by proxy through another transfer representation.

Deprecated

init(exporting: (Item) throws -> ProxyRepresentation, importing: (ProxyRepresentation) async throws -> Item)

Creates a transfer representation that’s imported and exported by proxy through another transfer representation.

init(importing: (ProxyRepresentation) async throws -> Item)

Creates a transfer representation that’s imported by proxy through another transfer representation.

init(importing: (ProxyRepresentation) throws -> Item)

Creates a transfer representation that’s imported by proxy through another transfer representation.

### Type Aliases

typealias Body

The transfer representation for the item.

### Default Implementations

TransferRepresentation Implementations

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### Transfer customization

struct TransferRepresentationVisibility

The visibility levels that specify the kinds of apps and processes that can see an item in transit.

