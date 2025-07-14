

- Core Transferable
- ProxyRepresentation
-  init(importing:) 

Initializer

# init(importing:)

Creates a transfer representation that’s imported by proxy through another transfer representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(importing: @escaping (ProxyRepresentation) throws -> Item)
```

## Parameters 

`importing`  

A closure that converts the chosen representation into the transported item.

