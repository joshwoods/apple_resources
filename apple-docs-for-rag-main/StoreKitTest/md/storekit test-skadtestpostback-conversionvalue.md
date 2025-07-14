

- StoreKit Test
- SKAdTestPostback
-  conversionValue 

Instance Property

# conversionValue

An unsigned 6-bit value that the app or ad network controls.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var conversionValue: Int { get }
```

## Discussion

A postback in SKAdNetwork 3 or earlier uses a single conversionValue. A postback in SKAdNetwork 4 or later may contain either a fineConversionValue or a coarseConversionValue.

## See Also

### Getting information in earlier versions

var adCampaignIdentifier: Int

A number that represents the advertising network’s campaign.

