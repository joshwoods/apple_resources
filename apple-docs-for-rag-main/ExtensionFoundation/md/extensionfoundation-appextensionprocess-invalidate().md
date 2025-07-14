

- ExtensionFoundation
- AppExtensionProcess
-  invalidate() 

Instance Method

# invalidate()

Stop the extension process.

macOS 13.0+

``` source
func invalidate()
```

## Discussion

When you call this method, you tell the system your app no longer needs this extension process. If this is the last connection from the host process to the extension process, the system terminates the extension process.

## See Also

### Managing the Extension Process

func makeXPCConnection() throws -> NSXPCConnection

Creates a new XPC connection to the extension process.

