

- Virtualization
- VZVirtualMachineView
-  virtualMachine 

Instance Property

# virtualMachine

The VM to display in the view.

macOS 12.0+

``` source
@MainActor
var virtualMachine: VZVirtualMachine? { get set }
```

## See Also

### Configuring the VM

var automaticallyReconfiguresDisplay: Bool

A Boolean value that indicates whether the graphics display associated with this view automatically reconfigures with respect to view changes.

var capturesSystemKeys: Bool

A Boolean value that determines whether the system should send certain system keyboard shortcuts to the guest instead of the host.

