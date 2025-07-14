

- SKAdNetwork for Web Ads
-  AdImpressionResponse 

Object

# AdImpressionResponse

The response you provide that contains a signed payload for a clicked web ad.

SKAdNetwork for Web Ads 1.0+

``` source
object AdImpressionResponse
```

## Properties

`ad_network_id`

`string`

 (Required) 

The ad network ID.

You receive an ad network ID when you register to use SKAdNetwork. For more information, see Registering an ad network.

`itunes_item_id`

`integer`

 (Required) 

The App Store app ID that the ad impression advertises. This is the same value the ad network provides in the attributable ad link. For more information, see Creating an attributable ad link.

`nonce`

`string`

 (Required) 

This value needs to match the value of `source_nonce` in the AdImpressionRequest. The value needs to be in the `UUID` string format.

Provide the dash-separated representation of the `source_nonce`.

`signature`

signature

 (Required) 

The cryptographic signature the ad network generates to sign the web ad. For more information, see Generating a signature for attributable web ads.

`source_domain`

`string`

 (Required) 

The effective top-level domain and one more preceding path component (eTLD+1) representation of the ad network serving the ad. This value needs to match the `source_domain` value you receive in the AdImpressionRequest.

`source_identifier`

`integer`

 (Required) 

A four-digit value you use to measure the aspects of an advertising effort or campaign.

`timestamp`

`integer`

 (Required) 

An integer that represents the UNIX time, in milliseconds, that you create this AdImpressionResponse.

`version`

`string`

 (Required) 

The SKAdNetwork version. Use version `"4.0"` or later. For version information, see SKAdNetwork release notes.

## Attributes 

Possible types:

## Mentioned in 

Creating an attributable ad link

Generating a signature for attributable web ads

## Discussion

This is a response that you provide to the Get a Signed Web Ad Impression Payload endpoint. When you create an AdImpressionResponse, use the dash-separated string representation of the UUID, which you decode from the `source_nonce` in the AdImpressionRequest that you receive.

Important

The `attributionSourceNonce` in a web ad link, the `source_nonce` in an AdImpressionRequest, and the `nonce` in this response all represent the same UUID, but the encoding varies.

## See Also

### Providing the web ad signature and response

Generating a signature for attributable web ads

Initiate install-validation by providing the signed parameters for an attributable web ad.

object signature

The key-value pairs that ad networks use to cryptographically sign a web ad.

