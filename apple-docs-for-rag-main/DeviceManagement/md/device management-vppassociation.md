

- Device Management
-  VppAssociation 

Object

# VppAssociation

An association between a license and a user or device.

Device Assignment ServicesVPP License Management

``` source
object VppAssociation
```

## Properties

`clientUserIdStr`

`string`

The client-supplied identifier used when registering a user.

`errorMessage`

`string`

The human-readable explanation of the error.

`errorNumber`

`int32`

The numeric code of the error.

`licenseIdStr`

`string`

The license identifier assigned to a user or device.

`serialNumber`

`string`

The device serial number.

## See Also

### Objects and Data Types

object VppAsset

A particular asset in the purchase program.

object VppAssignment

An assignment’s properties and their values.

object VppLicense

A license for a product in the purchase program.

object VppUser

A user within the purchase program.

object VppLocation

A location used for managing purchases.

object VppErrorCode

An error code.

