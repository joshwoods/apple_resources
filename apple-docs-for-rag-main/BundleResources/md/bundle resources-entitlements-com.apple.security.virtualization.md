

- Bundle Resources
- Entitlements
-  com.apple.security.virtualization 

Property List Key

# com.apple.security.virtualization

A Boolean value that indicates whether your app can use the Virtualization framework.

macOS 11.0+

## Details 

Type  

boolean

## Discussion

You can read the `VZVirtualMachine` property isSupported to check for the availability of virtualization on the system. Calling validate() checks for the availability of the entitlement the framework requires to run guest OSes.

## See Also

### Hypervisor

com.apple.security.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

com.apple.vm.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

Deprecated

com.apple.vm.device-access

A Boolean value that indicates whether the app captures USB devices and uses them in the guest-operating system.

com.apple.vm.networking

A Boolean that indicates whether the app manages virtual network interfaces without escalating privileges to the root user.

