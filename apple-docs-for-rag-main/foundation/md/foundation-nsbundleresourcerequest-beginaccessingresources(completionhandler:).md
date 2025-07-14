

- Foundation
- NSBundleResourceRequest
-  beginAccessingResources(completionHandler:) 

Instance Method

# beginAccessingResources(completionHandler:)

Requests access to the resources marked with the managed tags. If any of the resources are not on the device, they are requested from the App Store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func beginAccessingResources(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func beginAccessingResources() async throws
```

## Parameters 

`completionHandler`  

A block called when the resources have finished downloading or if an error occurs. The resources are not available until the completion handler is called with `error` set to `nil`.

The block takes the following parameter:

error  
Set to `nil` if the resources are downloaded successfully; otherwise this parameter holds an NSError object describing the problem that occurred. Errors are usually due to a lack of free space or problems connecting with the App Store.

## Discussion

After calling this method, the resource request downloads any on-demand resources not already on the device. When all the resources are downloaded, they are marked as non-purgeable. The resources are not available to the app until the completion handler is called with no error.

Important

You must call this method or conditionallyBeginAccessingResources(completionHandler:) before accessing any resources marked with the tags managed by the request.

## See Also

### Requesting Resources

func conditionallyBeginAccessingResources(completionHandler: (Bool) -> Void)

Checks whether the resources marked with the tags managed by the request are already on the device. If all of the resources are on the device, you can begin accessing those resources.

func endAccessingResources()

Informs the system that you have finished accessing the resources marked with the tags managed by the request.

