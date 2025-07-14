

- Device Management
-  ManageAssetsRequest 

Object

# ManageAssetsRequest

The request for asset management.

Device Assignment ServicesVPP License Management

``` source
object ManageAssetsRequest
```

## Properties

`assets`

`[`Asset`]`

 (Required) 

The set of `adamId` and `pricingParam values`.

`clientUserIds`

`[string]`

The set of identifiers for users in your organization.

`serialNumbers`

`[string]`

The set of identifiers for devices in your organization.

## Mentioned in 

Managing Assets

## Topics

### Objects and Data Types

object Asset

A product in the store.

## See Also

### Request and Response

object EventResponse

The response that contains the event identifier.

object ErrorResponse

The response that contains the error that occurs.

