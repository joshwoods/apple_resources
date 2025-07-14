

- Bundle Resources
- Entitlements
-  com.apple.vm.hypervisor Deprecated

Property List Key

# com.apple.vm.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

macOS 10.10–11.0Deprecated

Deprecated

For apps with a deployment target of macOS 11 and later, use com.apple.security.hypervisor instead. For deployment targets earlier than macOS 11, add both that and the com.apple.vm.hypervisor entitlement to your app.

## Details 

Type  

boolean

## Discussion

The entitlement is required to use the Hypervisor APIs in a sandboxed process.

## See Also

### Hypervisor

com.apple.security.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

com.apple.vm.device-access

A Boolean value that indicates whether the app captures USB devices and uses them in the guest-operating system.

com.apple.vm.networking

A Boolean that indicates whether the app manages virtual network interfaces without escalating privileges to the root user.

com.apple.security.virtualization

A Boolean value that indicates whether your app can use the Virtualization framework.

