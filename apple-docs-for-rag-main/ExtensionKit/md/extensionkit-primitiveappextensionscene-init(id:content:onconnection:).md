

- ExtensionKit
- PrimitiveAppExtensionScene
-  init(id:content:onConnection:) 

Initializer

# init(id:content:onConnection:)

Creates a new app extension scene.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    id: String,
    @ViewBuilder content: @escaping () -> Content,
    onConnection: @escaping (NSXPCConnection) -> Bool = { _ in false }
) where Content : View
```

## Parameters 

`id`  

A unique identifier for the scene.

`content`  

The scene’s user interface.

`onConnection`  

A closure that runs when the extension connects to its host.

