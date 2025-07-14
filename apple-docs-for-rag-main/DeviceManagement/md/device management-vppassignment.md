

- Device Management
-  VppAssignment 

Object

# VppAssignment

An assignment’s properties and their values.

Device Assignment ServicesVPP License Management

``` source
object VppAssignment
```

## Properties

`adamIdStr`

`string`

The unique identifier for a product in the iTunes Store.

`clientUserIdStr`

`string`

The client user ID of the user that the device is currently assigned to.

`pricingParam`

`string`

The quality of a product in the iTunes Store. Possible values are:

- `STDQ`: Standard quality

- `PLUS`: High quality

`serialNumber`

`string`

The device’s serial number that the license is currently assigned to.

## See Also

### Objects and Data Types

object VppAsset

A particular asset in the purchase program.

object VppLicense

A license for a product in the purchase program.

object VppAssociation

An association between a license and a user or device.

object VppUser

A user within the purchase program.

object VppLocation

A location used for managing purchases.

object VppErrorCode

An error code.

