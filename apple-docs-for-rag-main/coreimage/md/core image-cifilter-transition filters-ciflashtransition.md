

- Core Image
- CIFilter
- Transition Filters
-  CIFlashTransition 

Protocol

# CIFlashTransition

The properties you use to configure a flash transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIFlashTransition
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var color: CIColor

The color of the light rays emanating from the flash.

**Required**

var extent: CGRect

The extent of the flash.

**Required**

var fadeThreshold: Float

The amount of fade between the flash and the target image.

**Required**

var maxStriationRadius: Float

The radius of the light rays emanating from the flash.

**Required**

var striationContrast: Float

The contrast of the light rays emanating from the flash.

**Required**

var striationStrength: Float

The strength of the light rays emanating from the flash.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func flashTransition() -> any CIFilter &amp; CIFlashTransition

Creates a flash of light to transition between two images.

