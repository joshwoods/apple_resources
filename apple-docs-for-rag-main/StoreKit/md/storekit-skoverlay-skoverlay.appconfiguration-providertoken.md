

- StoreKit
- SKOverlay
- SKOverlay.AppConfiguration
-  providerToken 

Instance Property

# providerToken

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var providerToken: String? { get set }
```

## Discussion

When you set a provider token, you must also set the campaignToken.

When promoting your own apps, set your own provider token using `providerToken`. This allows you to track a promotion’s effectiveness independently from any affiliate campaign that shares the same campaign token.

When promoting apps by other developers, set `providerToken` using their provider token. This allows those developers to track the effectiveness of your App Store Connect Analytics campaign.

## See Also

### Verifying Advertising Campaigns

var campaignToken: String?

A token you use to represent an ad campaign and measure its effectiveness.

func setAdditionalValue(Any?, forKey: String)

Sets an additional value for a key; for example, a value for measuring the effectiveness of an ad campaign.

func additionalValue(forKey: String) -> Any?

Returns the object associated with the key.

