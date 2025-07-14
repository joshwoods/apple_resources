

- AppKit
- NSColorSpaceName
-  named 

Type Property

# named

Catalog name and color name components

macOS

``` source
static let named: NSColorSpaceName
```

## Discussion

The components of this color space are indexes into lists or catalogs of prepared colors. The catalogs of named colors come with lookup tables that are able to generate the correct color on a given device.

## See Also

### Color Space Names

static let calibratedRGB: NSColorSpaceName

Calibrated color space with red, green, blue, and alpha components.

static let calibratedWhite: NSColorSpaceName

Calibrated color space with white and alpha components (pure white is 1.0)

static let custom: NSColorSpaceName

Custom `NSColorSpace` object and floating-point components describing a color in that space

static let deviceCMYK: NSColorSpaceName

Device-dependent color space with cyan, magenta, yellow, black, and alpha components

static let deviceRGB: NSColorSpaceName

Device-dependent color space with red, green, blue, and alpha components.

static let deviceWhite: NSColorSpaceName

Device-dependent color space with white and alpha components (pure white is 1.0)

static let pattern: NSColorSpaceName

Pattern image (tiled)

