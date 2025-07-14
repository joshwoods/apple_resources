

- Bundle Resources
- Entitlements
-  Communicates with Drivers 

Property List Key

# Communicates with Drivers

A Boolean value that indicates whether an iPadOS app can communicate with drivers.

iOS 16.0+iPadOS 16.0+

## Details 

Key  
com.apple.developer.driverkit.communicates-with-drivers

Type  

boolean

## Discussion

When `true`, this entitlement allows your app to open user clients to one or more drivers.

On macOS, use the com.apple.developer.driverkit.userclient-access entitlement instead.

## See Also

### User client entitlements

com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

com.apple.developer.driverkit.allow-any-userclient-access

A Boolean value that determines whether a macOS driver accepts user client connections from any application.

DriverKit Allow Third Party User Clients

A Boolean value that indicates whether an iPadOS driver accepts calls from third-party user clients.

**Key:** com.apple.developer.driverkit.allow-third-party-userclients

