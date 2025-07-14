

- Foundation
- NSFileProviderService
-  getFileProviderConnection(completionHandler:) 

Instance Method

# getFileProviderConnection(completionHandler:)

Asynchronously returns the service’s connection object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func getFileProviderConnection(completionHandler: @escaping (NSXPCConnection?, (any Error)?) -> Void)
```

``` source
func fileProviderConnection() async throws -> NSXPCConnection
```

## Parameters 

`completionHandler`  

A block that is called on an anonymous background queue. The system passes this block the following parameters:

`connection`  
An NSXPCConnection object for the service, or `nil` if an error occurs.

`error`  
If an error occurs, this property contains an object that describes the error; otherwise, it is set to `nil`.

## See Also

### Accessing the Service

var name: NSFileProviderServiceName

The File Provider service’s name.

