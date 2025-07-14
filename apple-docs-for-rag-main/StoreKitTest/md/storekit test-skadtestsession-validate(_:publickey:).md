

- StoreKit Test
- SKAdTestSession
-  validate(\_:publicKey:) 

Instance Method

# validate(\_:publicKey:)

Validates an impression for a view-through ad.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
func validate(
    _ impression: SKAdImpression,
    publicKey: String
) throws
```

## Parameters 

`impression`  

An SKAdImpression instance, representing your ad impression.

`publicKey`  

The public key of the elliptic curve cryptographic key pair you used to generate the signature for the ad impression.

## Discussion

The cryptographic key pair you use for testing may be a different key pair than you use in production. For testing, use keys from the same key pair to sign the ad impression for testing and call validate(_:publicKey:).

For more information about signing ad impressions, see Signing and providing ads.

## See Also

### Validating impressions

func validateImpression(parameters: [String : Any], publicKey: String) throws

Validates an impression for a StoreKit-rendered ad.

func validateWebAdImpressionPayload(Data, publicKey: String) throws

Validates an impression for a web ad.

