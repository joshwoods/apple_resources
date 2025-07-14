

- Core Image
- CIImage
-  Autoadjustment Keys 

API Collection

# Autoadjustment Keys

Constants used as keys in the options dictionary for the autoAdjustmentFilters(options:) method.

## Topics

### Constants

static let enhance: CIImageAutoAdjustmentOption

A key used to specify whether to return enhancement filters.

static let redEye: CIImageAutoAdjustmentOption

A key used to specify whether to return a red eye filter.

static let features: CIImageAutoAdjustmentOption

A key used to specify an array of features that you want to apply enhancement and red eye filters to.

static let crop: CIImageAutoAdjustmentOption

A key used to specify whether to return a filter that crops the image to focus on detected features.

static let level: CIImageAutoAdjustmentOption

A key used to specify whether to return a filter that rotates the image to keep a level perspective.

## See Also

### Getting Autoadjustment Filters

func autoAdjustmentFilters() -> [CIFilter]

Returns all possible automatically selected and configured filters for adjusting the image.

func autoAdjustmentFilters(options: [CIImageAutoAdjustmentOption : Any]?) -> [CIFilter]

Returns a subset of automatically selected and configured filters for adjusting the image.

