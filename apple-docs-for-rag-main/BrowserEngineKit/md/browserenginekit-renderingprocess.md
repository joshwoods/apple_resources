

- BrowserEngineKit
-  RenderingProcess 

Structure

# RenderingProcess

An object that represents a running browser rendering extension process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
struct RenderingProcess
```

## Mentioned in 

Managing the browser extension life cycle

## Overview

Your browser app may have one or more rendering extensions, which each need a separate bundle identifier. Your browser can launch one instance of each of its rendering extensions.

## Topics

### Creating and invalidating extension processes

init(bundleIdentifier: String?, onInterruption: () -> Void) async throws

Launches a rendering extension process asynchronously.

func invalidate()

Stops the extension process.

### Creating XPC connections

func makeLibXPCConnection() throws -> xpc_connection_t

Creates a new XPC connection to the extension process.

### Coordinating processes

func grantCapability(ProcessCapability) throws -> ProcessCapability.Grant

Grants the specified capability to the process.

func grantCapability(ProcessCapability, invalidationHandler: () -> Void) throws -> ProcessCapability.Grant

Grants the specified capability to the process, calling the handler when the capability becomes invalid.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the rendering process.

## See Also

### Host app representations

struct WebContentProcess

An object that represents a running web content extension process.

struct NetworkingProcess

An object that represents a running browser networking extension process.

