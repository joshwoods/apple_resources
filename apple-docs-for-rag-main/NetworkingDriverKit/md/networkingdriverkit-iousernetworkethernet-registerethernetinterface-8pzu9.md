

- NetworkingDriverKit
- IOUserNetworkEthernet
-  registerEthernetInterface 

Instance Method

# registerEthernetInterface

DriverKit 24.0+

``` source
IOReturn registerEthernetInterface(ether_addr_t macAddress, IOUserNetworkPacketQueue * * queues, uint32_t numQueues, IOUserNetworkPacketBufferPool * txPool, IOUserNetworkPacketBufferPool * rxPool);
```

