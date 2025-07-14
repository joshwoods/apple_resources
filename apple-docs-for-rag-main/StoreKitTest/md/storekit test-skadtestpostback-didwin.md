

- StoreKit Test
- SKAdTestPostback
-  didWin 

Instance Property

# didWin

A Boolean value that indicates whether the postback won the attribution.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var didWin: Bool { get }
```

## See Also

### Getting conversion information

var fidelityType: Int

An integer that indicates the type of ad impression, StoreKit-rendered or view-through.

var fineConversionValue: Int

The specific conversion value of an ad postback.

var coarseConversionValue: SKAdNetwork.CoarseConversionValue?

A value that indicates a high, medium, or low conversion value for an ad postback.

