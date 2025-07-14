

- Bundle Resources
- Entitlements
-  System Extension Entitlement 

Property List Key

# System Extension Entitlement

A Boolean value that indicates whether your app has permission to activate or deactivate system extensions.

macOS 10.15+

## Details 

Key  
com.apple.developer.system-extension.install

Type  

boolean

## Discussion

To add this entitlement to your app, enable the System Extension capability in Xcode. Add this entitlement for all system extension types, including DriverKit extensions.

## See Also

### Essentials

System Extension Redistributable Entitlement

A Boolean value that indicates whether other development teams may distribute a system extension you create.

**Key:** com.apple.developer.system-extension.redistributable

