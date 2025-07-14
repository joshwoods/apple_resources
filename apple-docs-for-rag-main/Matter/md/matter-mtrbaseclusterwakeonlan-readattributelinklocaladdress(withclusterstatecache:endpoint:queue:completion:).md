

- Matter
- MTRBaseClusterWakeOnLAN
-  readAttributeLinkLocalAddress(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeLinkLocalAddress(withClusterStateCache:endpoint:queue:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class func readAttributeLinkLocalAddress(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
class func readAttributeLinkLocalAddress(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> Data
```

