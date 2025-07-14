

- ExtensionFoundation
-  AppExtensionProcess 

Structure

# AppExtensionProcess

An object that represents a running app extension process.

macOS 13.0+

``` source
struct AppExtensionProcess
```

## Overview

The system guarantees that the extension process has launched by the time any init methods return. If the extension process exits, the system calls onInterruption on configuration object you passed to the init method.

## Topics

### Finding or Launching Extensions

init(configuration: AppExtensionProcess.Configuration) throws

Synchronously finds an existing extension process or launches a new one.

init(configuration: AppExtensionProcess.Configuration) async throws

Asynchronously finds an existing extension process or launches a one.

struct Configuration

An object that holds configuration options for an app extension process.

### Managing the Extension Process

func makeXPCConnection() throws -> NSXPCConnection

Creates a new XPC connection to the extension process.

func invalidate()

Stop the extension process.

