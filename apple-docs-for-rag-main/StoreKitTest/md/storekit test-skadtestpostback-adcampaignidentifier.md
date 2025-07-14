

- StoreKit Test
- SKAdTestPostback
-  adCampaignIdentifier 

Instance Property

# adCampaignIdentifier

A number that represents the advertising network’s campaign.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var adCampaignIdentifier: Int { get }
```

## Discussion

Ad networks set their own campaign identifiers, which must be an integer between 1 and 100.

## See Also

### Getting information in earlier versions

var conversionValue: Int

An unsigned 6-bit value that the app or ad network controls.

