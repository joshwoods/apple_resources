

- SKAdNetwork for Web Ads
-  signature 

Object

# signature

The key-value pairs that ad networks use to cryptographically sign a web ad.

SKAdNetwork for Web Ads 1.0+

``` source
object signature
```

## Properties

`version`

`string`

 (Required) 

The SKAdNetwork version. Use version `“4.0”` or later. For version information, see SKAdNetwork release notes.

`ad_network_id`

`string`

 (Required) 

The ad network ID.

You receive an ad network ID when you register to use SKAdNetwork. For more information, see Registering an ad network.

`source_identifier`

`integer`

 (Required) 

A four-digit value you use to measure the aspects of an advertising effort or campaign.

`itunes_item_id`

`integer`

 (Required) 

The App Store ID of the app that the ad impression advertises. This is the same value the ad network provides in the attributable ad link. For more information, see Creating an attributable ad link.

`nonce`

`string`

 (Required) 

A UUID you generate to include in the signature. This value needs to match the value of `attributionSourceNonce` in the original ad link. This value needs to be in the `UUID` string format.

Provide the dash-separated representation of the `attributionSourceNonce`.

`source_domain`

`string`

 (Required) 

The effective top-level domain and one more preceding path component (eTLD+1) representation of the ad network that seeks ad attribution.

`fidelity_type`

`integer`

 (Required) 

The fidelity type value for web ads is `1`.

`timestamp`

`integer`

 (Required) 

An integer that represents the UNIX time, in milliseconds, of the ad impression.

## Attributes 

Possible types:

## Mentioned in 

Generating a signature for attributable web ads

## Discussion

Use the required parameters in the signature object to generate a cryptographic signature for the AdImpressionResponse. For more information, see Generating a signature for attributable web ads.

## See Also

### Providing the web ad signature and response

Generating a signature for attributable web ads

Initiate install-validation by providing the signed parameters for an attributable web ad.

object AdImpressionResponse

The response you provide that contains a signed payload for a clicked web ad.

