

- Matter
- MTROTAProviderDelegate
-  handleBDXQuery(forNodeID:controller:blockSize:blockIndex:bytesToSkip:completion:) 

Instance Method

# handleBDXQuery(forNodeID:controller:blockSize:blockIndex:bytesToSkip:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
optional func handleBDXQuery(
    forNodeID nodeID: NSNumber,
    controller: MTRDeviceController,
    blockSize: NSNumber,
    blockIndex: NSNumber,
    bytesToSkip: NSNumber,
    completion: @escaping (Data?, Bool) -> Void
)
```

``` source
optional func handleBDXQuery(
    forNodeID nodeID: NSNumber,
    controller: MTRDeviceController,
    blockSize: NSNumber,
    blockIndex: NSNumber,
    bytesToSkip: NSNumber
) async -> (Data?, Bool)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func handleBDXQuery(forNodeID nodeID: NSNumber, controller: MTRDeviceController, blockSize: NSNumber, blockIndex: NSNumber, bytesToSkip: NSNumber) async -> (Data?, Bool)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

