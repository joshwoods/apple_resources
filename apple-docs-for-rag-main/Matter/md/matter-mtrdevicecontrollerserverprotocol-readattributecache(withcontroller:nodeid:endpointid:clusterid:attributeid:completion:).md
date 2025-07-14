

- Matter
- MTRDeviceControllerServerProtocol
-  readAttributeCache(withController:nodeId:endpointId:clusterId:attributeId:completion:) 

Instance Method

# readAttributeCache(withController:nodeId:endpointId:clusterId:attributeId:completion:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func readAttributeCache(
    withController controller: Any?,
    nodeId: UInt64,
    endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?,
    completion: @escaping MTRValuesHandler
)
```

``` source
func readAttributeCache(
    withController controller: Any?,
    nodeId: UInt64,
    endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?
) async throws -> Any
```

**Required**

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributeCache(withController controller: Any?, nodeId: UInt64, endpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?) async throws -> Any
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

