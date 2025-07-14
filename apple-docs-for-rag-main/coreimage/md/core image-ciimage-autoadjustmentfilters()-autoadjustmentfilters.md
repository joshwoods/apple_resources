

- Core Image
- CIImage
-  autoAdjustmentFilters() 

Instance Method

# autoAdjustmentFilters()

Returns all possible automatically selected and configured filters for adjusting the image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func autoAdjustmentFilters() -> [CIFilter]
```

## Return Value

An array of CIFilter instances preconfigured for correcting deficiencies in the supplied image.

## See Also

### Getting Autoadjustment Filters

func autoAdjustmentFilters(options: [CIImageAutoAdjustmentOption : Any]?) -> [CIFilter]

Returns a subset of automatically selected and configured filters for adjusting the image.

Autoadjustment Keys

Constants used as keys in the options dictionary for the autoAdjustmentFilters(options:) method.

