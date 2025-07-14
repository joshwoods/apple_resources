

- BrowserEngineKit
-  Extension lifecycle 

API Collection

# Extension lifecycle

Launch, communicate with, and invalidate browser extensions.

## Topics

### Essentials

Managing the browser extension life cycle

Coordinate helper processes to efficiently support your browser app.

Using XPC to communicate with browser extensions

Build interprocess communication between your host app and extensions.

### Browser extensions

protocol WebContentExtension

An interface for configuring a web content helper extension process that will carry web page decoding operations on behalf of the browser app.

struct WebContentExtensionConfiguration

protocol NetworkingExtension

An interface for configuring a networking helper extension process that will carry out networking operations on behalf of the browser app.

struct NetworkingExtensionConfiguration

protocol RenderingExtension

An interface for configuring a rendering helper extension process that will carry out operations requiring rendering access on behalf of the browser app.

struct RenderingExtensionConfiguration

### Host app representations

struct WebContentProcess

An object that represents a running web content extension process.

struct NetworkingProcess

An object that represents a running browser networking extension process.

struct RenderingProcess

An object that represents a running browser rendering extension process.

### Extension capabilities

enum ProcessCapability

An enumeration that identifies capabilities that a browser app can grant to its extension processes.

struct MediaEnvironment

An object that identifies a media playback or streaming environment.

## See Also

### Browser extensions

Creating browser extensions in Xcode

Configure your Xcode project to support your alternative browser engine.

Extension resources

Control access to files and memory in browser extensions.

