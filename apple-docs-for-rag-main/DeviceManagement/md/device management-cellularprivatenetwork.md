

- Device Management
-  CellularPrivateNetwork 

Device Management Profile

# CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

``` source
object CellularPrivateNetwork
```

## Properties

`CellularDataPreferred`

`boolean`

Set to `true` to prefer this private network over Wi-Fi.

Default: `false`

`CsgNetworkIdentifier`

`string`

`DataSetName`

`string`

 (Required) 

The name of the private network configuration data set.

`EnableNRStandalone`

`boolean`

Set to `true` if this private network is NR Standalone.

Default: `false`

`Geofences`

`[`CellularPrivateNetwork.GeofenceItem`]`

A list of up to 1000 geofences for private networks. Geofencing is only used on iPhone.

`NetworkIdentifier`

`string`

`VersionNumber`

`string`

 (Required) 

The version number of this dataset that the system uses to track updates.

## Discussion

Specify `com.apple.cellularprivatenetwork.managed` as the payload type.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Allow Manual Install       | iOS              |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | iOS              |
| Allow Multiple Payloads    | \-               |

### Profile Example

```

   PayloadContent

           CellularDataPreferred

           DataSetName
           ExamplePrivateNetwork
           EnableNRStandalone

           Geofences

                   Longitude
                   -122.009
                   Latitude
                   37.3346
                   Radius
                   200
                   GeofenceId
                   AppleParkGeofence

           VersionNumber
           1.0
           PayloadIdentifier
           com.example.cellularprivatenetwork
           PayloadDescription
           GeofenceData
           PayloadType
           com.apple.cellularprivatenetwork.managed
           PayloadUUID
           1d6d6912-708e-441a-9272-526ef05bbe3c
           PayloadVersion
           1

   PayloadDisplayName
   Cellular Private Network
   PayloadIdentifier
   com.example.myprofile
   PayloadType
   Configuration
   PayloadUUID
   3425E7C2-9B02-49EB-8818-F65AA36DDE83
   PayloadVersion
   1

```

## Topics

### Objects

object CellularPrivateNetwork.GeofenceItem

A geofence for a private network.

## See Also

### Networking

object Cellular

The payload you use to configure cellular settings.

object ContentCaching

The payload you use to configure the content-caching service.

object DNSSettings

The payload you use to configure encrypted DNS settings.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

