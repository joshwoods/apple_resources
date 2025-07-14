

- Matter
- MTRBaseClusterBasicInformation
-  readAttributeProductAppearance(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeProductAppearance(withClusterStateCache:endpoint:queue:completion:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class func readAttributeProductAppearance(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (MTRBasicInformationClusterProductAppearanceStruct?, (any Error)?) -> Void
)
```

``` source
class func readAttributeProductAppearance(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> MTRBasicInformationClusterProductAppearanceStruct
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func readAttributeProductAppearance(withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t) async throws -> MTRBasicInformationClusterProductAppearanceStruct
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

