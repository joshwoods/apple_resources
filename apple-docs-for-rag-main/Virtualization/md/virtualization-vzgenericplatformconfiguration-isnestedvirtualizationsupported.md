

- Virtualization
- VZGenericPlatformConfiguration
-  isNestedVirtualizationSupported 

Type Property

# isNestedVirtualizationSupported

A Boolean value that describes whether the platform configuration supports nested virtualization.

macOS 15.0+

``` source
class var isNestedVirtualizationSupported: Bool { get }
```

## Discussion

Important

Nested virtualization is available for Mac with the M3 chip, and later.

Use this property to check whether support is available for the platform. As the following example shows, if the framework supports nested virtualization on the host, use isNestedVirtualizationEnabled to enable the feature:

- Swift
- Objective-C

```
if needsNestedVirtualization && VZGenericPlatformConfiguration.isNestedVirtualizationSupported {
    genericPlatformConfiguration.isNestedVirtualizationEnabled = true
}
```

```
if (needsNestedVirtualization && VZGenericPlatformConfiguration.isNestedVirtualizationSupported) {
    genericPlatformConfiguration.nestedVirtualizationEnabled = YES;
}
```

## See Also

### Identifying the platform configuration

var machineIdentifier: VZGenericMachineIdentifier

A value that represents a unique identifier for the virtual machine.

var isNestedVirtualizationEnabled: Bool

A Boolean value that indicates whether nested virtualization is in an enabled state.

class VZGenericMachineIdentifier

An object that represents a unique identifier for a virtual machine.

