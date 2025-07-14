

- File Provider
- NSFileProviderServiceSource
-  makeListenerEndpoint() 

Instance Method

# makeListenerEndpoint()

Returns an endpoint object that lets the host app communicate with the File Provider extension.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func makeListenerEndpoint() throws -> NSXPCListenerEndpoint
```

**Required**

## See Also

### Accessing the Service

var serviceName: NSFileProviderServiceName

A name that uniquely identifies the service (reverse domain name notation is recommended).

**Required**

var isRestricted: Bool

