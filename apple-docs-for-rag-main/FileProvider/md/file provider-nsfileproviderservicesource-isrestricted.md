

- File Provider
- NSFileProviderServiceSource
-  isRestricted 

Instance Property

# isRestricted

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.0+

``` source
optional var isRestricted: Bool { get }
```

## See Also

### Accessing the Service

var serviceName: NSFileProviderServiceName

A name that uniquely identifies the service (reverse domain name notation is recommended).

**Required**

func makeListenerEndpoint() throws -> NSXPCListenerEndpoint

Returns an endpoint object that lets the host app communicate with the File Provider extension.

**Required**

