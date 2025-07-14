

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  readAttributeForecast(withClusterStateCache:endpoint:queue:completion:) 

Type Method

# readAttributeForecast(withClusterStateCache:endpoint:queue:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class func readAttributeForecast(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t,
    completion: @escaping (MTRDeviceEnergyManagementClusterForecastStruct?, (any Error)?) -> Void
)
```

``` source
class func readAttributeForecast(
    withClusterStateCache clusterStateCacheContainer: MTRClusterStateCacheContainer,
    endpoint: NSNumber,
    queue: dispatch_queue_t
) async throws -> MTRDeviceEnergyManagementClusterForecastStruct
```

