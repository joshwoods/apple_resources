

- Bundle Resources
- Entitlements
-  DriverKit Allow Third Party User Clients 

Property List Key

# DriverKit Allow Third Party User Clients

A Boolean value that indicates whether an iPadOS driver accepts calls from third-party user clients.

iOS 16.0+iPadOS 16.0+

## Details 

Key  
com.apple.developer.driverkit.allow-third-party-userclients

Type  

boolean

## Discussion

By default, an iPadOS driver accepts user-client connections from apps signed with the same team ID and the Communicates with Drivers entitlement. Set this entitlement to `true` on a driver to allow connections apps with other team IDs. The connecting apps must still have the Communicates with Drivers entitlement.

## See Also

### User client entitlements

com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

com.apple.developer.driverkit.allow-any-userclient-access

A Boolean value that determines whether a macOS driver accepts user client connections from any application.

Communicates with Drivers

A Boolean value that indicates whether an iPadOS app can communicate with drivers.

**Key:** com.apple.developer.driverkit.communicates-with-drivers

