

- NetworkingDriverKit
- IOUserNetworkTxSubmissionQueue
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

Don’t call this method directly. Instead, use the `IOUserNetworkTxSubmissionQueue/Create` method to create a new IOUserNetworkTxSubmissionQueue object.

## See Also

### Creating the Submission Queue

free

Performs any final cleanup for the queue.

