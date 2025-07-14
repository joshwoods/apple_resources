

- Vision
- BarcodeObservation
-  supplementalCompositeType 

Instance Property

# supplementalCompositeType

The supplemental composite type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let supplementalCompositeType: BarcodeObservation.CompositeType?
```

## Discussion

Currently, this can only refer to the composite flag of the 2D symbology as part of a GS1 composite symbology.

This attribute only exists when the primary descriptor is the 1D symbology of a GS1 composite symbology, and of which a valid 2D counterpart has been coalesced into.

## See Also

### Getting the composite type

enum CompositeType

Composite types for barcode requests.

