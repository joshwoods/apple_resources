

- BrowserEngineKit
- NetworkingExtensionConfiguration
-  accept(connection:) 

Instance Method

# accept(connection:)

A method the system calls when a host app tries to connect.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
nonisolated
func accept(connection: NSXPCConnection) -> Bool
```

## Parameters 

`connection`  

The connection requesting to connect.

## Return Value

A Boolean value indicating if you are accepting the request.

