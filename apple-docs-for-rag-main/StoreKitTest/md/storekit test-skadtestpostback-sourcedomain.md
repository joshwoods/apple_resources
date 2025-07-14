

- StoreKit Test
- SKAdTestPostback
-  sourceDomain 

Instance Property

# sourceDomain

The source of a web ad.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var sourceDomain: String? { get }
```

## Discussion

This postback value indicates the `source_domain` of the corresponding AdImpressionRequest.

## See Also

### Getting advertisement information

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

var appStoreItemIdentifier: Int

The item identifier of the app that this ad impression advertises.

var sourceAppStoreItemIdentifier: Int

The item identifier of the app that displays the ad.

var sourceIdentifier: String?

A string that identifies an ad campaign.

