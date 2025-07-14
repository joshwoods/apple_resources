

- StoreKit Test
- SKAdTestPostback
-  coarseConversionValue 

Instance Property

# coarseConversionValue

A value that indicates a high, medium, or low conversion value for an ad postback.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var coarseConversionValue: SKAdNetwork.CoarseConversionValue? { get }
```

## Discussion

A postback in SKAdNetwork version 4 and later provides a fineConversionValue or this coarseConversionValue. Earlier versions of SKAdNetwork use a single conversionValue.

## See Also

### Getting conversion information

var fidelityType: Int

An integer that indicates the type of ad impression, StoreKit-rendered or view-through.

var fineConversionValue: Int

The specific conversion value of an ad postback.

var didWin: Bool

A Boolean value that indicates whether the postback won the attribution.

