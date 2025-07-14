

- CarPlay
- CPRouteChoice
-  selectionSummaryVariants 

Instance Property

# selectionSummaryVariants

An array of selection summary variants.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var selectionSummaryVariants: [String]? { get }
```

## Discussion

When creating a CPRouteChoice object, localize each variant for display to the user. The system displays the first variant that fits in the available screen space, so arrange the variants from most to least preferred display order. The array contains at least one variant.

## See Also

### Getting Variants

var summaryVariants: [String]

An array of summary variants.

var additionalInformationVariants: [String]?

An array of variants providing additional information about the route choice.

