

- StoreKit
- SKOverlay
- SKOverlay.AppConfiguration
-  setAdditionalValue(\_:forKey:) 

Instance Method

# setAdditionalValue(\_:forKey:)

Sets an additional value for a key; for example, a value for measuring the effectiveness of an ad campaign.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func setAdditionalValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

The value to associate with the `key`.

`key`  

The string that identifies an additional value.

## Discussion

Set additional values to verify and associate an app installation with an ad campaign. For more information, see SKAdNetwork.

## See Also

### Verifying Advertising Campaigns

var campaignToken: String?

A token you use to represent an ad campaign and measure its effectiveness.

var providerToken: String?

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

func additionalValue(forKey: String) -> Any?

Returns the object associated with the key.

