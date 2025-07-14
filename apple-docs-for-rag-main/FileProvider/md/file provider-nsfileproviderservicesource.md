

- File Provider
-  NSFileProviderServiceSource 

Protocol

# NSFileProviderServiceSource

A service that provides a custom communication channel between the host app and the File Provider extension.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderServiceSource
```

## Overview

To implement a File Provider service, the NSFileProviderExtension subclass must override the supportedServiceSources(for:) method and return the supported services.

For more information about creating services, see NSFileProviderService.

## Topics

### Accessing the Service

var serviceName: NSFileProviderServiceName

A name that uniquely identifies the service (reverse domain name notation is recommended).

**Required**

func makeListenerEndpoint() throws -> NSXPCListenerEndpoint

Returns an endpoint object that lets the host app communicate with the File Provider extension.

**Required**

var isRestricted: Bool

## See Also

### Working with services

func supportedServiceSources(for: NSFileProviderItemIdentifier) throws -> [any NSFileProviderServiceSource]

Return an array of service sources that let the host app perform actions associated with the specified item.

