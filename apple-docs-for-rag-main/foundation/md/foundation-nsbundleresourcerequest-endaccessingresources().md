

- Foundation
- NSBundleResourceRequest
-  endAccessingResources() 

Instance Method

# endAccessingResources()

Informs the system that you have finished accessing the resources marked with the tags managed by the request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func endAccessingResources()
```

## Discussion

Call this method as soon as you have finished using the tags managed by this request. If needed, this method will be called by the system when the resource request object is deallocated.

Important

The callback from beginAccessingResources(completionHandler:) or conditionallyBeginAccessingResources(completionHandler:) must have completed before calling endAccessingResources().

## See Also

### Requesting Resources

func beginAccessingResources(completionHandler: ((any Error)?) -> Void)

Requests access to the resources marked with the managed tags. If any of the resources are not on the device, they are requested from the App Store.

func conditionallyBeginAccessingResources(completionHandler: (Bool) -> Void)

Checks whether the resources marked with the tags managed by the request are already on the device. If all of the resources are on the device, you can begin accessing those resources.

