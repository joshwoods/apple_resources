

- Bundle Resources
- Entitlements
-  System Extension Redistributable Entitlement 

Property List Key

# System Extension Redistributable Entitlement

A Boolean value that indicates whether other development teams may distribute a system extension you create.

macOS 10.15+

## Details 

Key  
com.apple.developer.system-extension.redistributable

Type  

boolean

## Discussion

Add this entitlement to a system extension that you create and sign using your development team credentials, but which other development teams distribute in their apps. This extension allows a distributing app to have a different team ID than the one associated with the system extension. If this entitlement isn’t present, the team ID of the app and system extension must match.

## See Also

### Essentials

System Extension Entitlement

A Boolean value that indicates whether your app has permission to activate or deactivate system extensions.

**Key:** com.apple.developer.system-extension.install

