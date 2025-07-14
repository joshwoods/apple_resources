

- ExtensionKit
- AppExtensionSceneConfiguration
-  accept(connection:) 

Instance Method

# accept(connection:)

A closure the framework calls when a host tries to connect to this extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func accept(connection: NSXPCConnection) -> Bool
```

## Parameters 

`connection`  

The incoming XPC connection object.

## Return Value

A boolean value that indicates whether the extension accepts the connection.

