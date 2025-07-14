

- Matter
- MTRBaseClusterTestCluster
-  readAttributeWriteOnlyInt8u(withAttributeCache:endpoint:queue:completionHandler:) Deprecated

Type Method

# readAttributeWriteOnlyInt8u(withAttributeCache:endpoint:queue:completionHandler:)

iOS 16.2–16.4DeprecatediPadOS 16.2–16.4DeprecatedMac Catalyst 16.2–16.4DeprecatedmacOS 13.1–13.3DeprecatedtvOS 16.2–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.2–9.4Deprecated

``` source
class func readAttributeWriteOnlyInt8u(
    withAttributeCache attributeCacheContainer: MTRAttributeCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completionHandler: @escaping (NSNumber?, (any Error)?) -> Void
)
```

``` source
class func readAttributeWriteOnlyInt8u(
    withAttributeCache attributeCacheContainer: MTRAttributeCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> NSNumber
```

Deprecated

Please use readAttributeWriteOnlyInt8uWithAttributeCache:endpoint:queue:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func readAttributeWriteOnlyInt8u(withAttributeCache attributeCacheContainer: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t) async throws -> NSNumber
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

