

- Core Media I/O
- CMIOExtensionProvider
-  init(source:clientQueue:) 

Initializer

# init(source:clientQueue:)

Creates an extension provider with the specified source and dispatch queue.

Mac Catalyst 15.4+macOS 12.3+

``` source
init(
    source: any CMIOExtensionProviderSource,
    clientQueue: dispatch_queue_t?
)
```

## Parameters 

`source`  

An extension-specific object that conforms to the CMIOExtensionProviderSource protocol.

`clientQueue`  

A client dispatch queue, or `nil` to use the default queue.

