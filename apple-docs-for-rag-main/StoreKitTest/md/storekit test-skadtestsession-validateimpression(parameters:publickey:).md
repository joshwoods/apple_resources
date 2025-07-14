

- StoreKit Test
- SKAdTestSession
-  validateImpression(parameters:publicKey:) 

Instance Method

# validateImpression(parameters:publicKey:)

Validates an impression for a StoreKit-rendered ad.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
func validateImpression(
    parameters: [String : Any],
    publicKey: String
) throws
```

## Parameters 

`parameters`  

A dictionary containing version-specific key values that associate an app installation with an ad campaign for StoreKit-rendered ads. See Ad network install-validation keys for the list of required keys.

`publicKey`  

The public key of the elliptic curve cryptographic key pair you used to generate the signature for the ad impression.

## Discussion

The cryptographic key pair you use for testing may be a different key pair than you use in production. For testing, use keys from the same key pair when you sign the ad impression and when you call validateImpression(parameters:publicKey:).

For more information about signing ad impressions, see Signing and providing ads.

## See Also

### Validating impressions

func validate(SKAdImpression, publicKey: String) throws

Validates an impression for a view-through ad.

func validateWebAdImpressionPayload(Data, publicKey: String) throws

Validates an impression for a web ad.

