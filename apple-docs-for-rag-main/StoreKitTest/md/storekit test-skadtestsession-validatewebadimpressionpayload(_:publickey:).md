

- StoreKit Test
- SKAdTestSession
-  validateWebAdImpressionPayload(\_:publicKey:) 

Instance Method

# validateWebAdImpressionPayload(\_:publicKey:)

Validates an impression for a web ad.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
func validateWebAdImpressionPayload(
    _ impressionData: Data,
    publicKey: String
) throws
```

## See Also

### Validating impressions

func validate(SKAdImpression, publicKey: String) throws

Validates an impression for a view-through ad.

func validateImpression(parameters: [String : Any], publicKey: String) throws

Validates an impression for a StoreKit-rendered ad.

