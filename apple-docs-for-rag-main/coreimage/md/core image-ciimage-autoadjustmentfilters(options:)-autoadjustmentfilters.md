

- Core Image
- CIImage
-  autoAdjustmentFilters(options:) 

Instance Method

# autoAdjustmentFilters(options:)

Returns a subset of automatically selected and configured filters for adjusting the image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func autoAdjustmentFilters(options: [CIImageAutoAdjustmentOption : Any]? = nil) -> [CIFilter]
```

## Parameters 

`options`  

You can control which filters are returned by supplying one or more of the keys described in Autoadjustment Keys.

The options dictionary can also contain a CIDetectorImageOrientation key. Because some autoadjustment filters rely on face detection, you should specify an image orientation if you want to enable these filters for an image containing face whose orientation does not match that of the image.

## Return Value

An array of CIFilter instances preconfigured for correcting deficiencies in the supplied image.

## See Also

### Getting Autoadjustment Filters

func autoAdjustmentFilters() -> [CIFilter]

Returns all possible automatically selected and configured filters for adjusting the image.

Autoadjustment Keys

Constants used as keys in the options dictionary for the autoAdjustmentFilters(options:) method.

