

- Foundation
- Progress
-  removeSubscriber(\_:) 

Type Method

# removeSubscriber(\_:)

Removes a proxy progress object that the add subscriber method returns.

macOS 10.9+

``` source
class func removeSubscriber(_ subscriber: Any)
```

## Parameters 

`subscriber`  

The proxy of the progress object to observe.

## Discussion

If the block for addSubscriber(forFileURL:withPublishingHandler:) returns a closure, the system invokes that closure on the main thread when you invoke removeSubscriber(_:).

## See Also

### Observing and Controlling File Progress by Other Processes

class func addSubscriber(forFileURL: URL, withPublishingHandler: Progress.PublishingHandler) -> Any

Registers a file URL to hear about the progress of a file operation.

var isOld: Bool

A Boolean value that indicates when the observed progress object invokes the publish method before you subscribe to it.

typealias PublishingHandler

A block that the system calls when an observed progress object matches the subscription.

typealias UnpublishingHandler

A block that the system calls when an observed progress object terminates the subscription.

