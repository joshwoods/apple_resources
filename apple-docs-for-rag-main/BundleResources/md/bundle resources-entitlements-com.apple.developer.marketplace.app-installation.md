

- Bundle Resources
- Entitlements
-  com.apple.developer.marketplace.app-installation 

Property List Key

# com.apple.developer.marketplace.app-installation

The entitlement that enables an app to vend other apps as an alternative app marketplace.

iOS 17.4+iPadOS 17.4+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

The system requires that your app have this entitlement to implement an app marketplace and install other apps using MarketplaceKit. Apple approves your use of this entitlement based on a set of criteria. To request the entitlement, see Getting started as an alternative app marketplace in the European Union. For more information, see Creating an alternative app marketplace.

If your account receives this entitlement, provision your app with the entitlement according to: Provisioning with managed capabilities.

Note

This entitlement isn’t available for Enterprise or Developer ID distributed apps.

