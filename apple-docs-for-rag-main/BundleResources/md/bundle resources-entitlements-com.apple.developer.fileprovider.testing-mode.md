

- Bundle Resources
- Entitlements
-  com.apple.developer.fileprovider.testing-mode 

Property List Key

# com.apple.developer.fileprovider.testing-mode

A Boolean value that indicates whether you can place domains in testing mode.

macOS 11.3+visionOS 1.0+

## Details 

Type  

boolean

## Discussion

You must add this entitlement to your target before assigning a non-empty value to a domain’s testingModes property. You can only use this entitlement during testing and development. If you add it to your app or extension, you must remove it before you submit your app to TestFlight or the Mac App Store.

