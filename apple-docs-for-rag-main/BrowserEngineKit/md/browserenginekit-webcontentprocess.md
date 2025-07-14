

- BrowserEngineKit
-  WebContentProcess 

Structure

# WebContentProcess

An object that represents a running web content extension process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
struct WebContentProcess
```

## Mentioned in 

Managing the browser extension life cycle

## Overview

A web browser app may launch multiple web content extension processes, and each instance of this object represents a separate process.

## Topics

### Creating and invalidating extension processes

init(bundleIdentifier: String?, onInterruption: () -> Void) async throws

Launches a web content process asynchronously.

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

Returns an interaction that associates a view with the web content process.

## See Also

### Host app representations

struct NetworkingProcess

An object that represents a running browser networking extension process.

struct RenderingProcess

An object that represents a running browser rendering extension process.

