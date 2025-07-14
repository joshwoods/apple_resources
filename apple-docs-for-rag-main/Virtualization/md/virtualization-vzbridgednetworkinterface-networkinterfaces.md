

- Virtualization
- VZBridgedNetworkInterface
-  networkInterfaces 

Type Property

# networkInterfaces

The bridged network interfaces that you may use in your virtual machine.

macOS 11.0+

``` source
class var networkInterfaces: [VZBridgedNetworkInterface] { get }
```

## Discussion

The system creates the objects in this property based on the available interfaces in the host machine.

