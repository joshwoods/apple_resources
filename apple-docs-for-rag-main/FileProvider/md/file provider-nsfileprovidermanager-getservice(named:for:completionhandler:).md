

- File Provider
- NSFileProviderManager
-  getService(named:for:completionHandler:) 

Instance Method

# getService(named:for:completionHandler:)

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.0+

``` source
func getService(
    named serviceName: NSFileProviderServiceName,
    for itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping (NSFileProviderService?, (any Error)?) -> Void
)
```

``` source
func service(
    named serviceName: NSFileProviderServiceName,
    for itemIdentifier: NSFileProviderItemIdentifier
) async throws -> NSFileProviderService?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func service(named serviceName: NSFileProviderServiceName, for itemIdentifier: NSFileProviderItemIdentifier) async throws -> NSFileProviderService?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

