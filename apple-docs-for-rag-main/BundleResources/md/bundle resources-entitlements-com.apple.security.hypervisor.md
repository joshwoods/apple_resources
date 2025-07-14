

- Bundle Resources
- Entitlements
-  com.apple.security.hypervisor 

Property List Key

# com.apple.security.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

macOS 11.0+

## Details 

Type  

boolean

## Discussion

The entitlement is required to use the Hypervisor APIs in any process.

Important

If your app has a deployment target of macOS 10.15 or earlier, add the com.apple.vm.hypervisor entitlement to your app in addition to this entitlement.

## See Also

### Hypervisor

com.apple.vm.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

Deprecated

com.apple.vm.device-access

A Boolean value that indicates whether the app captures USB devices and uses them in the guest-operating system.

com.apple.vm.networking

A Boolean that indicates whether the app manages virtual network interfaces without escalating privileges to the root user.

com.apple.security.virtualization

A Boolean value that indicates whether your app can use the Virtualization framework.

