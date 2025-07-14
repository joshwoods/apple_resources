

- Virtualization
- VZVirtualMachineView
-  capturesSystemKeys 

Instance Property

# capturesSystemKeys

A Boolean value that determines whether the system should send certain system keyboard shortcuts to the guest instead of the host.

macOS 12.0+

``` source
@MainActor
var capturesSystemKeys: Bool { get set }
```

## Discussion

Defaults to `false.`

## See Also

### Configuring the VM

var automaticallyReconfiguresDisplay: Bool

A Boolean value that indicates whether the graphics display associated with this view automatically reconfigures with respect to view changes.

var virtualMachine: VZVirtualMachine?

The VM to display in the view.

