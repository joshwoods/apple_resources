

- Matter
- MTRBaseClusterGeneralCommissioning
-  readAttributeBasicCommissioningInfo(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeBasicCommissioningInfo(withClusterStateCache:endpoint:queue:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class func readAttributeBasicCommissioningInfo(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (MTRGeneralCommissioningClusterBasicCommissioningInfo?, (any Error)?) -> Void
)
```

``` source
class func readAttributeBasicCommissioningInfo(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> MTRGeneralCommissioningClusterBasicCommissioningInfo
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func readAttributeBasicCommissioningInfo(withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t) async throws -> MTRGeneralCommissioningClusterBasicCommissioningInfo
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

