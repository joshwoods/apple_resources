

- Device Management
-  ResponseAsset 

Object

# ResponseAsset

The asset that the organization owns.

Device Assignment ServicesVPP License Management

``` source
object ResponseAsset
```

## Properties

`adamId`

`string`

The unique identifier for the product in the store.

`assignedCount`

`int32`

The assigned amount of the asset.

`availableCount`

`int32`

The available amount of the asset.

`deviceAssignable`

`boolean`

The flag denoting whether the asset is device-assignable.

`pricingParam`

`string`

The quality of the product in the store.

Possible Values: `STDQ, PLUS`

`productType`

`string`

The asset product type.

Possible Values: `App, Book`

`retiredCount`

`int32`

The retired amount of the asset.

`revocable`

`boolean`

The flag denoting whether the asset is revocable.

`totalCount`

`int32`

The total amount of the asset.

`supportedPlatforms`

`[string]`

The platforms that the asset supports.

Possible Values: `iOS, macOS, tvOS, watchOS`

## Mentioned in 

Managing Assets

## See Also

### Objects and Data Types

object Asset

A product in the store.

object Assignment

The asset assignment for a user or device.

object RequestUser

The requested user in the organization.

object ResponseUser

The user in the organization.

