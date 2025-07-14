

- Foundation
- Progress
-  Progress.UnpublishingHandler 

Type Alias

# Progress.UnpublishingHandler

A block that the system calls when an observed progress object terminates the subscription.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias UnpublishingHandler = () -> Void
```

## See Also

### Observing and Controlling File Progress by Other Processes

class func addSubscriber(forFileURL: URL, withPublishingHandler: Progress.PublishingHandler) -> Any

Registers a file URL to hear about the progress of a file operation.

class func removeSubscriber(Any)

Removes a proxy progress object that the add subscriber method returns.

var isOld: Bool

A Boolean value that indicates when the observed progress object invokes the publish method before you subscribe to it.

typealias PublishingHandler

A block that the system calls when an observed progress object matches the subscription.

