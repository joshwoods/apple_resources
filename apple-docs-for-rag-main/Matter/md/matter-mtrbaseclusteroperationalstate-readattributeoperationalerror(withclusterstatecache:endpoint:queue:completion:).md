

- Matter
- MTRBaseClusterOperationalState
-  readAttributeOperationalError(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeOperationalError(withClusterStateCache:endpoint:queue:completion:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
class func readAttributeOperationalError(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (MTROperationalStateClusterErrorStateStruct?, (any Error)?) -> Void
)
```

``` source
class func readAttributeOperationalError(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> MTROperationalStateClusterErrorStateStruct
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func readAttributeOperationalError(withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t) async throws -> MTROperationalStateClusterErrorStateStruct
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

