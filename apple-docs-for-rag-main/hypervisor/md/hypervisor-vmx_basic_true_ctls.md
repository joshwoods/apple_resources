

- Hypervisor
-  VMX_BASIC_TRUE_CTLS 

Global Variable

# VMX_BASIC_TRUE_CTLS

This bit field, in the value returned by the IA32_VMX_BASIC model specific register, determines if it’s possible to disable any VMX controls.

macOS

``` source
var VMX_BASIC_TRUE_CTLS: UInt { get }
```

## Discussion

The hardware must return this bit as a 1 in order to create any VM using the framework.

