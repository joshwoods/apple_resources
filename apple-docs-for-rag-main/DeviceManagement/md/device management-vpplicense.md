

- Device Management
-  VppLicense 

Object

# VppLicense

A license for a product in the purchase program.

Device Assignment ServicesVPP License Management

``` source
object VppLicense
```

## Properties

`adamId`

`int64`

The unique identifier for a product in the iTunes Store.

`adamIdStr`

`string`

The unique identifier for a product in the iTunes Store.

`clientUserIdStr`

`string`

The client user ID for the user to whom this license is assigned.

`isIrrevocable`

`boolean`

If true, once a license is assigned for specified adamId, the license may not be revoked or disassociated.

`itsIdHash`

`string`

The hash of the iTunes Store ID for the user to whom this license is assigned. The itsIdHash field is included only when the user is associated with an iTunes Store account.

`licenseIdStr`

`string`

The identifier of the assigned license.

`pricingParam`

`string`

The quality of a product in the iTunes Store. Possible values are:

- `STDQ`: Standard quality

- `PLUS`: High quality

`productTypeId`

`int32`

The type of a product. Possible values are:

- `7` = macOS software

- `8` = iOS or macOS app from the App Store

- `10` = Book

`productTypeName`

`string`

The name of the product type.

`serialNumber`

`string`

The device serial number to which this license is assigned.

`status`

`string`

The current state of the license. Possible values are:

- `Associated`

- `Available`

- `Refunded`

`userId`

`int64`

The unique identifier assigned by the VPP for the user to whom this license is assigned.

`userIdStr`

`string`

The string representation of the unique identifier assigned by the VPP for the user to whom this license is assigned.

## See Also

### Objects and Data Types

object VppAsset

A particular asset in the purchase program.

object VppAssignment

An assignment’s properties and their values.

object VppAssociation

An association between a license and a user or device.

object VppUser

A user within the purchase program.

object VppLocation

A location used for managing purchases.

object VppErrorCode

An error code.

