

- Bundle Resources
- Entitlements
-  System Extensions 

API Collection

# System Extensions

Extend the capabilities of macOS from user space.

## Topics

### Essentials

System Extension Entitlement

A Boolean value that indicates whether your app has permission to activate or deactivate system extensions.

**Key:** com.apple.developer.system-extension.install

System Extension Redistributable Entitlement

A Boolean value that indicates whether other development teams may distribute a system extension you create.

**Key:** com.apple.developer.system-extension.redistributable

### Endpoint Security

com.apple.developer.endpoint-security.client

The entitlement required to monitor system events for potentially malicious activity.

### Human Interface Device Drivers

com.apple.developer.driverkit.family.hid.device

A Boolean value that indicates whether the driver provides a HID-related service to the system.

com.apple.developer.driverkit.family.hid.eventservice

A Boolean value that indicates whether the driver provides a HID-related event service to the system.

com.apple.developer.driverkit.transport.hid

A Boolean value that indicates whether the driver communicates with human interface devices.

com.apple.developer.hid.virtual.device

A Boolean value that indicates whether the driver creates a virtual HID device.

## See Also

### System

DriverKit

Develop device drivers in macOS and iPadOS.

