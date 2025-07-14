

- CarPlay
- CPLaneGuidance
-  instructionVariants 

Instance Property

# instructionVariants

An array of strings that represent the instruction for this lane guidance, arranged from most- to least-preferred.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var instructionVariants: [String] { get set }
```

## Discussion

You need to provide at least one variant. Provide the variant strings as localized, displayable content.

## See Also

### Properties

var lanes: [CPLane]

An array of lane objects, each describing a single lane.

