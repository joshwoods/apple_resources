

- Foundation
- NSFileProviderService
-  name 

Instance Property

# name

The File Provider service’s name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var name: NSFileProviderServiceName { get }
```

## See Also

### Accessing the Service

func getFileProviderConnection(completionHandler: (NSXPCConnection?, (any Error)?) -> Void)

Asynchronously returns the service’s connection object.

