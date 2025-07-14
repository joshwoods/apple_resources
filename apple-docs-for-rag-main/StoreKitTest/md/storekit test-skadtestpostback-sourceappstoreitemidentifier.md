

- StoreKit Test
- SKAdTestPostback
-  sourceAppStoreItemIdentifier 

Instance Property

# sourceAppStoreItemIdentifier

The item identifier of the app that displays the ad.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var sourceAppStoreItemIdentifier: Int { get }
```

## Discussion

In the testing environment, the sourceAppStoreItemIdentifier is always `0`.

## See Also

### Getting advertisement information

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

var appStoreItemIdentifier: Int

The item identifier of the app that this ad impression advertises.

var sourceDomain: String?

The source of a web ad.

var sourceIdentifier: String?

A string that identifies an ad campaign.

