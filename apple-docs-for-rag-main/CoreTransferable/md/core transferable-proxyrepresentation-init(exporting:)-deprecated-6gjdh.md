

- Core Transferable
- ProxyRepresentation
-  init(exporting:) Deprecated

Initializer

# init(exporting:)

Creates a transfer representation that’s exported by proxy through another transfer representation.

iOS 16.1–17.0DeprecatediPadOS 16.1–17.0DeprecatedMac Catalyst 16.1–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.1–17.0DeprecatedvisionOS 1.0+watchOS 9.1–10.0Deprecated

``` source
init(exporting: @escaping (Item) async throws -> ProxyRepresentation)
```

Deprecated

A synchronous exporter should be used instead.

## Parameters 

`exporting`  

A closure that converts the item into desired representation.

