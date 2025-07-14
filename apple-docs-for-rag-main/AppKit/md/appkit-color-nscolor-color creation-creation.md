

- AppKit
- Color
- NSColor
-  Color Creation 

API Collection

# Color Creation

Load colors from asset catalogs, and create colors from raw component values, such as those used by grayscale, RGB, HSB, and CMYK colors.

## Topics

### Loading Color Objects from Asset Catalogs

init?(named: NSColor.Name)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the app’s main bundle.

init?(named: NSColor.Name, bundle: Bundle?)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the specified bundle.

init?(catalogName: NSColorList.Name, colorName: NSColor.Name)

Creates a color object using the specified asset catalog and color names.

typealias Name

The name of a color.

### Creating a Color Using RGB Components

init(srgbRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the sRGB colorspace.

init(displayP3Red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object from the specified components in the Display P3 color space.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object with the specified red, green, blue, and alpha channel values.

init(calibratedRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and RGB components.

init(deviceRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and RGB components.

### Creating a Color Using HSB Components

init(calibratedHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and HSB color space components.

init(deviceHue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and HSB color space components.

init(hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object with the specified hue, saturation, brightness, and alpha channel values.

init(colorSpace: NSColorSpace, hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object with the specified color space, hue, saturation, brightness, and alpha channel values.

### Creating a Color Using CMYK Components

init(deviceCyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity value and CMYK components.

### Creating a Color Using White Components

init(white: CGFloat, alpha: CGFloat)

Creates a color object with the specified brightness and alpha channel values.

init(calibratedWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(deviceWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(genericGamma22White: CGFloat, alpha: CGFloat)

Returns a color object with the specified white and alpha values in the GenericGamma22 colorspace.

### Creating a Pattern-Based Color

init(patternImage: NSImage)

Creates a color object that uses the specified image pattern to paint the target area.

var patternImage: NSImage

The pattern image used to paint the target area.

### Creating a Color Dynamically

init(name: NSColor.Name?, dynamicProvider: (NSAppearance) -> NSColor)

Creates a dynamic catalog color with a provider that’s used to resolve the exact color value, calculated on first use.

### Creating a Color in an Arbitrary Color Space

init(colorSpace: NSColorSpace, components: UnsafePointer&lt;CGFloat>, count: Int)

Creates a color object from the specified components of the given color space.

### Creating a System Tint Color

init(for: NSControlTint)

Returns the color object specified by the given control tint.

Deprecated

enum NSControlTint

Constants for specifying a cell’s tint color.

### Converting Other Types of Color Objects

convenience init(Color)

init?(cgColor: CGColor)

Creates a color object using the specified Core Graphics color.

init(CIColor: CIColor)

Creates a color object from the specified Core Image color.

### Creating Color Objects

init()

Initializes the color object.

init?(coder: NSCoder)

Creates a color object from data in an unarchiver.

convenience init(resource: ColorResource)

## See Also

### Getting and Creating Colors

UI Element Colors

Retrieve standard color objects for use with windows, controls, labels, text, selections and other content in your app.

Standard Colors

Retrieve the standard color objects for common colors like red, blue, green, black, white, and more.

