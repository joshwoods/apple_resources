

- BrowserEngineKit
- NetworkingExtension
-  handle(xpcConnection:) 

Instance Method

# handle(xpcConnection:)

Accept or reject an incoming XPC connection.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func handle(xpcConnection: xpc_connection_t)
```

**Required**

## Parameters 

`xpcConnection`  

The inbound connection.

## Overview

When your browser app calls makeLibXPCConnection(), `BrowserEngineKit` calls this method on your extension, passing the newly created connection as the parameter. To accept the connection, call xpc_connection_set_event_handler(_:_:) to install an event handler and listen for incoming messages.

Otherwise, call xpc_connection_cancel(_:) to reject the connection.

