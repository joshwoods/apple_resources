

- StoreKit
- SKOverlay
- SKOverlay.AppClipConfiguration
-  campaignToken 

Instance Property

# campaignToken

A token you use to represent an ad campaign and measure its effectiveness.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var campaignToken: String? { get set }
```

## Discussion

A campaign token is a 40-byte string that represents an ad campaign. By setting the `campaignToken`, you can measure the effectiveness of an Apple Services Performance Partners Program link or an App Store Connect Analytics campaign.

For more information, see Apple Services Performance Partners Program and App Store Connect.

## See Also

### Verifying Advertising Campaigns

var providerToken: String?

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

func setAdditionalValue(Any?, forKey: String)

Sets an additional value for a key, such as a value for measuring the effectiveness of an ad campaign.

func additionalValue(forKey: String) -> Any?

Returns the object associated with the key.

