

- SKAdNetwork for Web Ads
-  AdImpressionRequest 

Object

# AdImpressionRequest

The request body that devices send to fetch the web ad impression from the ad network’s server.

SKAdNetwork for Web Ads 1.0+

``` source
object AdImpressionRequest
```

## Properties

`source_domain`

`string`

 (Required) 

The effective top-level domain and one more preceding path component (eTLD+1) representation of the ad network that seeks ad attribution.

`source_engagement_type`

`string`

 (Required) 

A key that describes the type of user action that leads to the ad impression. The value is `"click_to_App_Store"`.

`source_nonce`

`string`

 (Required) 

A Base64URL-encoded string representation of a UUID. This value is the same value the ad network provides as the `attributionSourceNonce` in the attributable ad link.

`version`

`string`

 (Required) 

The SKAdNetwork version of `"4.0"` or later. See SKAdNetwork release notes for version information.

## Attributes 

Possible types:

## Mentioned in 

Creating an attributable ad link

## Discussion

The device generates the AdImpressionRequest and sends it in the body of a Get a Signed Web Ad Impression Payload request. The device uses the value from the `attributionSourceNonce` in a web ad link for the `source_nonce` value in this request. The ad network looks up the fully signed web ad impression using the `source_nonce` value, which it creates when it serves the attributable ad link.

Important

The `attributionSourceNonce` in a web ad, the `source_nonce` in this request, and the `nonce` in a corresponding AdImpressionResponse all represent the same UUID, but the encoding varies.

## See Also

### Receiving a request for a web ad payload

Get a Signed Web Ad Impression Payload

An endpoint you provide to receive requests from devices to serve signed ad interactions.

