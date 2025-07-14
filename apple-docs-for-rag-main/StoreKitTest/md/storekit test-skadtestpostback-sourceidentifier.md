

- StoreKit Test
- SKAdTestPostback
-  sourceIdentifier 

Instance Property

# sourceIdentifier

A string that identifies an ad campaign.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var sourceIdentifier: String? { get }
```

## Discussion

The source identifier in a winning postback may contain two, three, or all four digits of the sourceIdentifier in the corresponding ad impression. For more information about the value you may get in the postback, see Receiving postbacks in multiple conversion windows.

## See Also

### Getting advertisement information

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

var appStoreItemIdentifier: Int

The item identifier of the app that this ad impression advertises.

var sourceAppStoreItemIdentifier: Int

The item identifier of the app that displays the ad.

var sourceDomain: String?

The source of a web ad.

