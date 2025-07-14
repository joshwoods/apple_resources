

- Virtualization
- VZBridgedNetworkDeviceAttachment
-  init(interface:) 

Initializer

# init(interface:)

Creates the attachment from a bridged network interface object.

macOS 11.0+

``` source
init(interface: VZBridgedNetworkInterface)
```

## Parameters 

`interface`  

An existing network interface of the host computer. Get a list of available interfaces from the networkInterfaces property of VZBridgedNetworkInterface.

## Return Value

An attachment object for the specified network interface.

