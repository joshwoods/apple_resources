

- Matter
- MTROTAProviderDelegate
-  handleQueryImage(forNodeID:controller:params:completion:) 

Instance Method

# handleQueryImage(forNodeID:controller:params:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
optional func handleQueryImage(
    forNodeID nodeID: NSNumber,
    controller: MTRDeviceController,
    params: MTROTASoftwareUpdateProviderClusterQueryImageParams,
    completion: @escaping (MTROTASoftwareUpdateProviderClusterQueryImageResponseParams?, (any Error)?) -> Void
)
```

``` source
optional func handleQueryImage(
    forNodeID nodeID: NSNumber,
    controller: MTRDeviceController,
    params: MTROTASoftwareUpdateProviderClusterQueryImageParams
) async throws -> MTROTASoftwareUpdateProviderClusterQueryImageResponseParams
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func handleQueryImage(forNodeID nodeID: NSNumber, controller: MTRDeviceController, params: MTROTASoftwareUpdateProviderClusterQueryImageParams) async throws -> MTROTASoftwareUpdateProviderClusterQueryImageResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

