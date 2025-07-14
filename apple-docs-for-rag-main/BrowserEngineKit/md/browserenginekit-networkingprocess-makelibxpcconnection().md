

- BrowserEngineKit
- NetworkingProcess
-  makeLibXPCConnection() 

Instance Method

# makeLibXPCConnection()

Creates a new XPC connection to the extension process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func makeLibXPCConnection() throws -> xpc_connection_t
```

## Return Value

An object that represents the new XPC connection.

## Overview

When you create an xpc_connection_t in your browser app using this method, the operating system calls your extension’s handle(xpcConnection:) method to supply the remote end of the connection to your extension process.

