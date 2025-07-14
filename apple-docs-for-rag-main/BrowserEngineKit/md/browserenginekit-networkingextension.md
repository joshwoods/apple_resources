

- BrowserEngineKit
-  NetworkingExtension 

Protocol

# NetworkingExtension

An interface for configuring a networking helper extension process that will carry out networking operations on behalf of the browser app.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
protocol NetworkingExtension : RestrictedSandboxAppliable, AppExtension
```

## Overview

When you add an object that conforms to `NetworkingExtension` in your extension’s Xcode target, annotate the conforming object with `@main` to indicate to `BrowserEngineKit` that this object is the entry point for your extension.

## Topics

### Handling incoming XPC connections

func handle(xpcConnection: xpc_connection_t)

Accept or reject an incoming XPC connection.

**Required**

## Relationships

### Inherits From

- AppExtension
- RestrictedSandboxAppliable

## See Also

### Browser extensions

protocol WebContentExtension

An interface for configuring a web content helper extension process that will carry web page decoding operations on behalf of the browser app.

struct WebContentExtensionConfiguration

struct NetworkingExtensionConfiguration

protocol RenderingExtension

An interface for configuring a rendering helper extension process that will carry out operations requiring rendering access on behalf of the browser app.

struct RenderingExtensionConfiguration

