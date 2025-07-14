

- Core Transferable
- ProxyRepresentation
-  init(exporting:importing:) 

Initializer

# init(exporting:importing:)

Creates a transfer representation that’s imported and exported by proxy through another transfer representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    exporting: @escaping (Item) throws -> ProxyRepresentation,
    importing: @escaping (ProxyRepresentation) throws -> Item
)
```

## Parameters 

`exporting`  

A closure that converts the item into desired representation.

`importing`  

A closure that converts the chosen representation back into the transported item.

