

- Bundle Resources
- Entitlements
-  Matter Allow Setup Payload 

Property List Key

# Matter Allow Setup Payload

A Boolean value that allows an app to provide an optional Matter Setup payload while setting up a Matter device in an ecosystem.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

## Details 

Key  
com.apple.developer.matter.allow-setup-payload

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

You may use this entitlement in the following ways:

- For adding a device that doesn’t have a Matter QR code to your ecosystem or Apple Home.

- For adding an already-paired Matter device from your ecosystem to Apple Home.

- For creating apps that have a built-in QR code scanner and have the ability to scan non-Matter QR codes.

If the caller provides the setup payload, the framework doesn’t show the user interface for QR code selection.

## See Also

### Home automation

HomeKit Entitlement

A Boolean value that indicates whether users of the app may manage HomeKit-compatible accessories.

**Key:** com.apple.developer.homekit

