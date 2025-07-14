

- NetworkingDriverKit
- IOUserNetworkPacket
-  init 

Instance Method

# init

Initializes the network packet object.

DriverKit

``` source
bool init();
```

## Return Value

`YES` if initialization was successful, or `NO` if it wasn’t.

## Discussion

Do not call this method directly. Submission queues initialize packets before returning them to your driver to process.

## See Also

### Configuring the Network Packet

free

Performs any final cleanup for the network packet.

