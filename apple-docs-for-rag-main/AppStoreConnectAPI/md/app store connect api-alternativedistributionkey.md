

- App Store Connect API
-  AlternativeDistributionKey 

Object

# AlternativeDistributionKey

The data structure that represents an alternative distribution key resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionKey
```

## Properties

`attributes`

AlternativeDistributionKey.Attributes

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the alternative distribution key.

`links`

ResourceLinks

`type`

`string`

 (Required) 

Value: `alternativeDistributionKeys`

## Discussion

For more information about the response that includes this alternative distribution key object, see AlternativeDistributionKeyResponse.

## Topics

### Objects

object AlternativeDistributionKey.Attributes

Attributes that describe an alternative distribution key resource.

## See Also

### Objects

object AlternativeDistributionKeyResponse

A response that contains a single alternative distribution key resource.

object AlternativeDistributionKeysResponse

A response that contains a list of alternative distribution keys.

object AlternativeDistributionKeyCreateRequest

The request body you use to create an alternative distribution key.

