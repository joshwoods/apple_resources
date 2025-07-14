

- PHASE
- PHASEBlendNodeDefinition
-  addRangeForInputValuesAbove(value:fullGainAtValue:fadeCurveType:subtree:) 

Instance Method

# addRangeForInputValuesAbove(value:fullGainAtValue:fadeCurveType:subtree:)

Adds a child node that blends above a given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func addRangeForInputValuesAbove(
    value: Double,
    fullGainAtValue: Double,
    fadeCurveType: PHASECurveType,
    subtree: PHASESoundEventNodeDefinition
)
```

## Parameters 

`value`  

The value below which the child node blends.

`fullGainAtValue`  

A threshold such that the node applies a fade curve to the child node’s gain when the blend parameter is between `value` and this value.

`fadeCurveType`  

An option that determines a rate of change for the child node’s gain over the fade range.

`subtree`  

A child node to blend.

## See Also

### Adding Child Nodes

func addRange(envelope: PHASEEnvelope, subtree: PHASESoundEventNodeDefinition)

Adds a child node with an envelope.

func addRangeForInputValuesBelow(value: Double, fullGainAtValue: Double, fadeCurveType: PHASECurveType, subtree: PHASESoundEventNodeDefinition)

Adds a child node that blends below a given value.

func addRangeForInputValuesBetween(lowValue: Double, highValue: Double, fullGainAtLowValue: Double, fullGainAtHighValue: Double, lowFadeCurveType: PHASECurveType, highFadeCurveType: PHASECurveType, subtree: PHASESoundEventNodeDefinition)

Adds a child node that blends between a given high and low value.

