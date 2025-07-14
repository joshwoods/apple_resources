

- Core Transferable
- ProxyRepresentation
-  init(importing:) 

Initializer

# init(importing:)

Creates a transfer representation that’s imported by proxy through another transfer representation.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
init(importing: @escaping (ProxyRepresentation) async throws -> Item)
```

## Parameters 

`importing`  

A closure that converts the chosen representation into the transported item.

