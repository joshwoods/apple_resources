

- File Provider
- NSFileProviderServiceSource
-  serviceName 

Instance Property

# serviceName

A name that uniquely identifies the service (reverse domain name notation is recommended).

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
var serviceName: NSFileProviderServiceName { get }
```

**Required**

## See Also

### Accessing the Service

func makeListenerEndpoint() throws -> NSXPCListenerEndpoint

Returns an endpoint object that lets the host app communicate with the File Provider extension.

**Required**

var isRestricted: Bool

