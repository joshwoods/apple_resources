

- Virtualization
- VZVirtualMachineDelegate
-  virtualMachine(\_:networkDevice:attachmentWasDisconnectedWithError:) 

Instance Method

# virtualMachine(\_:networkDevice:attachmentWasDisconnectedWithError:)

The method the framework calls when an error causes a VM’s network attachment to disconnect.

macOS 12.0+

``` source
optional func virtualMachine(
    _ virtualMachine: VZVirtualMachine,
    networkDevice: VZNetworkDevice,
    attachmentWasDisconnectedWithError error: any Error
)
```

## Parameters 

`virtualMachine`  

The VM invoking the delegate method.

`networkDevice`  

The disconnected network device.

`error`  

The error that describes why the virtual machine disconnected the network device.

## Discussion

The system invokes this method when the network interface fails to start, which results in the disconnection of the network attachment. This can happen in many situations such as initial boot, device reset, reboot, and so on. The system may invoke this method several times during a VM’s life cycle. After the system calls this method, the attachment property is `nil`.

