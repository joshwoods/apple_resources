

- NetworkingDriverKit
- IOUserNetworkRxSubmissionQueue
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

Don’t call this method directly. Instead, use the Create method to create a new IOUserNetworkRxSubmissionQueue object.

## See Also

### Creating the Submission Queue

Create

Creates a queue that delivers empty packets for you to fill with data from your hardware device.

free

Performs any final cleanup for the queue.

