

- Foundation
- Progress
-  isOld 

Instance Property

# isOld

A Boolean value that indicates when the observed progress object invokes the publish method before you subscribe to it.

macOS 10.9+

``` source
var isOld: Bool { get }
```

## Discussion

The publish and subscribe mechanism is generally *level-triggered*, in that when you invoke addSubscriber(forFileURL:withPublishingHandler:), the system invokes your block for every relevant published and unpublished progress object. Sometimes you need to implement *edge-triggered* behavior, in which you do something either exactly when new progress begins or not at all.

In the example above, the Dock doesn’t animate file icons when this method returns true.

There’s no reliable definition of *before* in this case, which involves multiple processes in a preemptively scheduled system. Don’t use this method for anything more important than best efforts at animating. It can be inaccurate due to processes coming and going from unpredictable user actions.

## See Also

### Observing and Controlling File Progress by Other Processes

class func addSubscriber(forFileURL: URL, withPublishingHandler: Progress.PublishingHandler) -> Any

Registers a file URL to hear about the progress of a file operation.

class func removeSubscriber(Any)

Removes a proxy progress object that the add subscriber method returns.

typealias PublishingHandler

A block that the system calls when an observed progress object matches the subscription.

typealias UnpublishingHandler

A block that the system calls when an observed progress object terminates the subscription.

