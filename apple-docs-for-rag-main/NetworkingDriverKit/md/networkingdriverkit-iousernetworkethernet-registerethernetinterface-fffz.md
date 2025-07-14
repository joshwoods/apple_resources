

- NetworkingDriverKit
- IOUserNetworkEthernet
-  RegisterEthernetInterface 

Instance Method

# RegisterEthernetInterface

DriverKit 21.0+

``` source
kern_return_t RegisterEthernetInterface(ether_addr_t macAddress, IOUserNetworkPacketBufferPool * pool, IOUserNetworkPacketQueue * * queues, uint32_t queueCount);
```

