

- Foundation
- Progress
-  addSubscriber(forFileURL:withPublishingHandler:) 

Type Method

# addSubscriber(forFileURL:withPublishingHandler:)

Registers a file URL to hear about the progress of a file operation.

macOS 10.9+

``` source
class func addSubscriber(
    forFileURL url: URL,
    withPublishingHandler publishingHandler: @escaping Progress.PublishingHandler
) -> Any
```

## Parameters 

`url`  

The URL of the file to observe.

`publishingHandler`  

A closure that the system invokes when a progress object that represents a file operation matching the specified URL calls publish().

## Return Value

A proxy of the progress object to observe.

## Discussion

The system invokes the passed-in block when a progress object calls publish() with a fileURLKey user info dictionary entry that’s a URL that is the same as this method’s URL, or that is an item that the URL directly contains. The progress object that passes to your block is a proxy of the published progress object. The passed-in block may return another block. If it does, the system invokes the returned block when the observed progress object invokes unpublish(), the publishing process terminates, or you invoke removeSubscriber(_:). The system invokes the blocks you provide on the main thread.

## See Also

### Observing and Controlling File Progress by Other Processes

class func removeSubscriber(Any)

Removes a proxy progress object that the add subscriber method returns.

var isOld: Bool

A Boolean value that indicates when the observed progress object invokes the publish method before you subscribe to it.

typealias PublishingHandler

A block that the system calls when an observed progress object matches the subscription.

typealias UnpublishingHandler

A block that the system calls when an observed progress object terminates the subscription.

