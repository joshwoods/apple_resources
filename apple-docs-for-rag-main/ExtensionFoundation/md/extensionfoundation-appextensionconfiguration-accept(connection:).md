

- ExtensionFoundation
- AppExtensionConfiguration
-  accept(connection:) 

Instance Method

# accept(connection:)

A method the system calls when a host app tries to connect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 9.0+

``` source
nonisolated
func accept(connection: NSXPCConnection) -> Bool
```

**Required**

## Parameters 

`connection`  

The connection requesting to connect.

## Return Value

A Boolean value indicating if you are accepting the request.

