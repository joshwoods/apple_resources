

- Matter
- MTRBaseClusterActions
-  readAttributeAttributeList(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeAttributeList(withClusterStateCache:endpoint:queue:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class func readAttributeAttributeList(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping ([Any]?, (any Error)?) -> Void
)
```

``` source
class func readAttributeAttributeList(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> [Any]
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func readAttributeAttributeList(withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t) async throws -> [Any]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

