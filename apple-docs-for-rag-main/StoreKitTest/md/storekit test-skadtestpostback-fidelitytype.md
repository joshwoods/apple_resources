

- StoreKit Test
- SKAdTestPostback
-  fidelityType 

Instance Property

# fidelityType

An integer that indicates the type of ad impression, StoreKit-rendered or view-through.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var fidelityType: Int { get set }
```

## Discussion

SKAdNetwork versions 2.2 and later require a fidelityType parameter for ad validation signatures. For view-through ads, use a fidelity type value of `0`. For StoreKit-rendered ads, use the value `1`.

## See Also

### Getting conversion information

var fineConversionValue: Int

The specific conversion value of an ad postback.

var coarseConversionValue: SKAdNetwork.CoarseConversionValue?

A value that indicates a high, medium, or low conversion value for an ad postback.

var didWin: Bool

A Boolean value that indicates whether the postback won the attribution.

