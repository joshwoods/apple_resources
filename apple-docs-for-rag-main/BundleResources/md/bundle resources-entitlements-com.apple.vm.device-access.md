

- Bundle Resources
- Entitlements
-  com.apple.vm.device-access 

Property List Key

# com.apple.vm.device-access

A Boolean value that indicates whether the app captures USB devices and uses them in the guest-operating system.

macOS 10.10+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

The entitlement is required to use the IOUSBHost APIs for USB device capture.

## See Also

### Hypervisor

com.apple.security.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

com.apple.vm.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

Deprecated

com.apple.vm.networking

A Boolean that indicates whether the app manages virtual network interfaces without escalating privileges to the root user.

com.apple.security.virtualization

A Boolean value that indicates whether your app can use the Virtualization framework.

