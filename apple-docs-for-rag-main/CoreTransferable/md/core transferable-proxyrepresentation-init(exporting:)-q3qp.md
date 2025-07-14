

- Core Transferable
- ProxyRepresentation
-  init(exporting:) 

Initializer

# init(exporting:)

Creates a transfer representation that’s exported by proxy through another transfer representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(exporting: @escaping (Item) throws -> ProxyRepresentation)
```

## Parameters 

`exporting`  

A closure that converts the item into desired representation.

