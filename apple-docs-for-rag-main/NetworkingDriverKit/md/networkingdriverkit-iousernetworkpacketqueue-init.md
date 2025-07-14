

- NetworkingDriverKit
- IOUserNetworkPacketQueue
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

Don’t call this method directly. Instead, use the Create method of the appropriate subclass.

## See Also

### Configuring the Packet Queue

free

Performs any final cleanup for the queue.

