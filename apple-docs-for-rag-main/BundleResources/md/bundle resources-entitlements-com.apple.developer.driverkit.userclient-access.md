

- Bundle Resources
- Entitlements
-  com.apple.developer.driverkit.userclient-access 

Property List Key

# com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

macOS 10.15+

## Details 

Type  

array of strings

## Discussion

Add this entitlement to your app that opens the IOUserClient. Set its value to an array of bundle IDs of driver extensions that you want to use with DriverKit. If you have only one bundle ID, you can use either a single string or a one-element array.

On iPadOS, use the Communicates with Drivers entitlement instead.

## See Also

### User client entitlements

com.apple.developer.driverkit.allow-any-userclient-access

A Boolean value that determines whether a macOS driver accepts user client connections from any application.

Communicates with Drivers

A Boolean value that indicates whether an iPadOS app can communicate with drivers.

**Key:** com.apple.developer.driverkit.communicates-with-drivers

DriverKit Allow Third Party User Clients

A Boolean value that indicates whether an iPadOS driver accepts calls from third-party user clients.

**Key:** com.apple.developer.driverkit.allow-third-party-userclients

