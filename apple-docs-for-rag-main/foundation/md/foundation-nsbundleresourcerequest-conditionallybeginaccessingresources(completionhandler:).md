

- Foundation
- NSBundleResourceRequest
-  conditionallyBeginAccessingResources(completionHandler:) 

Instance Method

# conditionallyBeginAccessingResources(completionHandler:)

Checks whether the resources marked with the tags managed by the request are already on the device. If all of the resources are on the device, you can begin accessing those resources.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func conditionallyBeginAccessingResources(completionHandler: @escaping (Bool) -> Void)
```

``` source
func conditionallyBeginAccessingResources() async -> Bool
```

## Parameters 

`completionHandler`  

A block called when the availability of the resources has been checked.

The block takes the following parameter:

resourcesAvailable  
Returns true if all of the resources marked with the tags managed by the request are already on the device. Returns false if any of the resources are not on the device.

## Discussion

If the resources marked with the tags managed by the request are already on the device, you can start accessing them as soon as the completion handler is called with `resourcesAvailable` set to true. If all of the resources are not already available, you need to call beginAccessingResources(completionHandler:) to download them from the App Store.

Important

If `resourcesAvailable` is true, do not call beginAccessingResources(completionHandler:). You must call this method or beginAccessingResources(completionHandler:) before accessing any resources marked with the tags managed by the request.

## See Also

### Requesting Resources

func beginAccessingResources(completionHandler: ((any Error)?) -> Void)

Requests access to the resources marked with the managed tags. If any of the resources are not on the device, they are requested from the App Store.

func endAccessingResources()

Informs the system that you have finished accessing the resources marked with the tags managed by the request.

