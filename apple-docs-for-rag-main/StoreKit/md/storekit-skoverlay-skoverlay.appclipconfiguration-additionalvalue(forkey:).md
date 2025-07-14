

- StoreKit
- SKOverlay
- SKOverlay.AppClipConfiguration
-  additionalValue(forKey:) 

Instance Method

# additionalValue(forKey:)

Returns the object associated with the key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func additionalValue(forKey key: String) -> Any?
```

## Parameters 

`key`  

The string that identifies an additional value.

## Return Value

The associated value of the key.

## Discussion

Additional values are values you use to verify and associate an app installation with an ad campaign. For more information, see SKAdNetwork.

## See Also

### Verifying Advertising Campaigns

var campaignToken: String?

A token you use to represent an ad campaign and measure its effectiveness.

var providerToken: String?

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

func setAdditionalValue(Any?, forKey: String)

Sets an additional value for a key, such as a value for measuring the effectiveness of an ad campaign.

