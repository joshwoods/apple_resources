

- ExtensionFoundation
- AppExtensionProcess
-  makeXPCConnection() 

Instance Method

# makeXPCConnection()

Creates a new XPC connection to the extension process.

macOS 13.0+

``` source
func makeXPCConnection() throws -> NSXPCConnection
```

## Return Value

The connection object representing the created XPC connection.

## Discussion

This method creates a connection to the extension process and returns it. You’re responsible for configuring the connection. While you retain a reference to the returned connection object, the extension receives processing time. Once you deallocate the connection object, the system suspends or terminates the extension process.

## See Also

### Managing the Extension Process

func invalidate()

Stop the extension process.

