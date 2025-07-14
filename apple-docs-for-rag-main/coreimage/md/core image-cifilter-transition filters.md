

- Core Image
- CIFilter
-  Transition Filters 

API Collection

# Transition Filters

## Topics

### Filters

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

class func barsSwipeTransition() -> any CIFilter &amp; CIBarsSwipeTransition

Transitions between two images by removing rectangular portions of an image.

class func copyMachineTransition() -> any CIFilter &amp; CICopyMachineTransition

Simulates the effect of a copy machine scanner light to transiton between two images.

class func disintegrateWithMaskTransition() -> any CIFilter &amp; CIDisintegrateWithMaskTransition

Transitions between two images using a mask image.

class func dissolveTransition() -> any CIFilter &amp; CIDissolveTransition

Transitions between two images with a fade effect.

class func flashTransition() -> any CIFilter &amp; CIFlashTransition

Creates a flash of light to transition between two images.

class func modTransition() -> any CIFilter &amp; CIModTransition

Transitions between two images by applying irregularly shaped holes.

class func pageCurlTransition() -> any CIFilter &amp; CIPageCurlTransition

Simulates the curl of a page, revealing the target image.

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

### Protocols

protocol CITransitionFilter

The properties you use to configure a transition filter.

protocol CIBarsSwipeTransition

The properties you use to configure a bars swipe transition filter.

protocol CIAccordionFoldTransition

The properties you use to configure an accordion fold transition filter.

protocol CICopyMachineTransition

The properties you use to configure a copy machine transition filter.

protocol CIDisintegrateWithMaskTransition

The properties you use to configure a disintegrate-with-mask transition filter.

protocol CIDissolveTransition

The properties you use to configure a dissolve transition filter.

protocol CIFlashTransition

The properties you use to configure a flash transition filter.

protocol CIModTransition

The properties you use to configure a mod transition filter.

protocol CIPageCurlTransition

The properties you use to configure a page curl transition filter.

protocol CIPageCurlWithShadowTransition

The properties you use to configure a page-curl-with-shadow transition filter.

protocol CIRippleTransition

The properties you use to configure a ripple transition filter.

protocol CISwipeTransition

The properties you use to configure a swipe transition filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

