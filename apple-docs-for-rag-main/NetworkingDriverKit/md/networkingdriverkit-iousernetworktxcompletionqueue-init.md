

- NetworkingDriverKit
- IOUserNetworkTxCompletionQueue
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

Don’t call this method directly. Instead, use the Create method to create a new IOUserNetworkTxCompletionQueue object.

## See Also

### Creating the Completion Queue

Create

Creates a queue that tells the system which packets you transmitted to your device.

free

Performs any final cleanup for the queue.

