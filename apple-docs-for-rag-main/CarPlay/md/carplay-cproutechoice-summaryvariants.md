

- CarPlay
- CPRouteChoice
-  summaryVariants 

Instance Property

# summaryVariants

An array of summary variants.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var summaryVariants: [String] { get }
```

## Discussion

When creating the CPRouteChoice object, localize each variant for display to the user. The system displays the first variant that fits into the available screen space, so arrange the variants from most to least preferred display order. The array contains at least one variant.

An example variant summary is *Via I-280 South.*

## See Also

### Getting Variants

var additionalInformationVariants: [String]?

An array of variants providing additional information about the route choice.

var selectionSummaryVariants: [String]?

An array of selection summary variants.

