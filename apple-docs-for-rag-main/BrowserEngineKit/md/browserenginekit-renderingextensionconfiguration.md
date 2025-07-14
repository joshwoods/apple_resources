

- BrowserEngineKit
-  RenderingExtensionConfiguration 

Structure

# RenderingExtensionConfiguration

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
@MainActor @preconcurrency
struct RenderingExtensionConfiguration
```

## Topics

### Instance Methods

func accept(connection: NSXPCConnection) -> Bool

A method the system calls when a host app tries to connect.

## Relationships

### Conforms To

- AppExtensionConfiguration
- Sendable

## See Also

### Browser extensions

protocol WebContentExtension

An interface for configuring a web content helper extension process that will carry web page decoding operations on behalf of the browser app.

struct WebContentExtensionConfiguration

protocol NetworkingExtension

An interface for configuring a networking helper extension process that will carry out networking operations on behalf of the browser app.

struct NetworkingExtensionConfiguration

protocol RenderingExtension

An interface for configuring a rendering helper extension process that will carry out operations requiring rendering access on behalf of the browser app.

