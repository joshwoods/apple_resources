

- Paravirtualized Graphics
- PGDisplayDescriptor
-  queue 

Instance Property

# queue

The queue that the framework uses when dispatching messages to any of the display’s registered handlers.

Mac Catalyst 14.0+macOS 11.0+

``` source
var queue: dispatch_queue_t? { get set }
```

## Discussion

Most often, your app provides a serial queue. If you can benefit from dispatching events out of order, handle the messages on the serial queue and redispatch them to other queues as necessary.

