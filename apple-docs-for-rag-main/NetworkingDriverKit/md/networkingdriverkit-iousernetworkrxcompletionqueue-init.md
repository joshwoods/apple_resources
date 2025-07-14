

- NetworkingDriverKit
- IOUserNetworkRxCompletionQueue
-  init 

Instance Method

# init

Initializes the packet submission queue.

DriverKit

``` source
bool init();
```

## Return Value

`YES` if initialization was successful, or `NO` if it wasn’t.

## Discussion

Don’t call this method directly. Instead, use the Create method to create a new IOUserNetworkRxCompletionQueue object.

## See Also

### Creating the Completion Queue

Create

Creates a queue that you use to deliver packets received from your hardware device.

free

Performs any final cleanup for the queue.

