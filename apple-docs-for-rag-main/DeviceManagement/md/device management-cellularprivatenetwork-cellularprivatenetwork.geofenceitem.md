

- Device Management
- CellularPrivateNetwork
-  CellularPrivateNetwork.GeofenceItem 

Device Management Profile

# CellularPrivateNetwork.GeofenceItem

A geofence for a private network.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

``` source
object CellularPrivateNetwork.GeofenceItem
```

## Properties

`GeofenceId`

`string`

 (Required) 

A geofence identifier that’s unique within a list of geofences.

`Latitude`

`number`

 (Required) 

The latitude of the geofence.

Minimum: `-90`

Maximum: `90`

`Longitude`

`number`

 (Required) 

The longitude of the geofence.

Minimum: `-180`

Maximum: `180`

`Radius`

`number`

 (Required) 

Specifies the radius of the geofence in meters. Set this value slightly greater than the private cellular network coverage area.

Minimum: `100`

Maximum: `6500`

## Discussion

Geofencing is only used on iPhone.

