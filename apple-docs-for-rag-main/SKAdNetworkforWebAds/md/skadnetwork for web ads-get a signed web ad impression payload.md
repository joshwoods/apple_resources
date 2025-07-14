

- SKAdNetwork for Web Ads
-  Get a Signed Web Ad Impression Payload 

Web Service Endpoint

# Get a Signed Web Ad Impression Payload

An endpoint you provide to receive requests from devices to serve signed ad interactions.

SKAdNetwork for Web Ads 1.0+

## URL

``` source
POST https://example.com/.well-known/skadnetwork/get-signed-payload
```

## HTTP Body

AdImpressionRequest

The request that devices send to this endpoint, asking for the web ad impression from the ad network’s server.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdImpressionResponse

`OK`

The response you provide that contains a signed payload for the clicked web ad.

Content-Type: application/json

## Mentioned in 

Creating an attributable ad link

Generating a signature for attributable web ads

## Discussion

You implement this endpoint on your server to provide signed SKAdNetwork ad payloads for web ads that users tap. The device calls this endpoint when a user taps an SKAdNetwork-attributable web ad.

To receive requests at this endpoint, your server needs to support the Transport Layer Security (TLS) 1.2 protocol or later.

The following is an example of an AdImpressionRequest payload:

```
```

A corresponding AdImpressionResponse to send in response to this payload is as follows:

```
```

Important

The `attributionSourceNonce` in a web ad, the `source_nonce` in an AdImpressionRequest, and the `nonce` in an AdImpressionResponse all represent the same UUID, but the encoding varies.

The device uses the same encoding as `attributionSourceNonce` for the `source_nonce` value in the AdImpressionRequest. However, you use the dash-separated string representation of the UUID for the `nonce` value in an AdImpressionResponse.

## See Also

### Receiving a request for a web ad payload

object AdImpressionRequest

The request body that devices send to fetch the web ad impression from the ad network’s server.

