

- File Provider
- NSFileProviderExternalVolumeHandling
-  shouldConnectExternalDomain(completionHandler:) 

Instance Method

# shouldConnectExternalDomain(completionHandler:)

Determines whether to connect to a domain from another device.

macOS 15.0+

``` source
func shouldConnectExternalDomain(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func shouldConnectExternalDomain() async throws
```

**Required**

