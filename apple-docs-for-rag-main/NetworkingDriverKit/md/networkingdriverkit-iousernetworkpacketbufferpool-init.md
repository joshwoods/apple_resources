

- NetworkingDriverKit
- IOUserNetworkPacketBufferPool
-  init 

Instance Method

# init

Initializes the network packet buffer pool object.

DriverKit

``` source
bool init();
```

## Return Value

`YES` if initialization was successful, or `NO` if an error occurred.

## See Also

### Creating a Buffer Pool

Create

Creates a new packet buffer pool object and allocates space for the specified number of packets.

free

Releases the resources owned by the network packet buffer pool object.

