

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetInterfaceEnable 

Instance Method

# SetInterfaceEnable

Enables or disables your service.

DriverKit

``` source
kern_return_t SetInterfaceEnable(bool isEnable);
```

## Parameters 

`isEnable`  

A Boolean value that indicates whether to enable or disable your service. Specify `YES` to enable the service or `NO` to disable it.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Override this method and use it to start or stop the delivery of packets to and from the device. For example, change the enabled state of the queues you use to handle packets moving to or from the device.

