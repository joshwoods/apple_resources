

- Matter
- MTRBaseClusterMessages
-  readAttributeMessages(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeMessages(withClusterStateCache:endpoint:queue:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class func readAttributeMessages(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping ([Any]?, (any Error)?) -> Void
)
```

``` source
class func readAttributeMessages(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> [Any]
```

