

- Matter
- MTRBaseClusterWaterHeaterManagement
-  readAttributeTankPercentage(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeTankPercentage(withClusterStateCache:endpoint:queue:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class func readAttributeTankPercentage(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (NSNumber?, (any Error)?) -> Void
)
```

``` source
class func readAttributeTankPercentage(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> NSNumber
```

