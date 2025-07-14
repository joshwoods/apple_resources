

- UIKit
- Drawing
- UIColor
-  Standard colors 

API Collection

# Standard colors

Define standard color objects for specific shades, such as red, blue, green, black, white, and more.

## Overview

Use the standard color objects when you want to use a specific color shade in your UI. To view swatches of these colors, see System Colors.

The system color objects adapt automatically to Dark Mode changes when you use the provided UIColor object, but the fixed-shade colors don’t adapt. If you retrieve the color values, either directly or using another type such as CGColor, you must handle Dark Mode changes yourself. For more information about supporting Dark Mode, see Supporting Dark Mode in Your Interface.

## Topics

### Adaptable colors

class var systemBlue: UIColor

A blue color that automatically adapts to the current trait environment.

class var systemBrown: UIColor

A brown color that automatically adapts to the current trait environment.

class var systemCyan: UIColor

A cyan color that automatically adapts to the current trait environment.

class var systemGreen: UIColor

A green color that automatically adapts to the current trait environment.

class var systemIndigo: UIColor

An indigo color that automatically adapts to the current trait environment.

class var systemMint: UIColor

A mint color that automatically adapts to the current trait environment.

class var systemOrange: UIColor

An orange color that automatically adapts to the current trait environment.

class var systemPink: UIColor

A pink color that automatically adapts to the current trait environment.

class var systemPurple: UIColor

A purple color that automatically adapts to the current trait environment.

class var systemRed: UIColor

A red color that automatically adapts to the current trait environment.

class var systemTeal: UIColor

A teal color that automatically adapts to the current trait environment.

class var systemYellow: UIColor

A yellow color that automatically adapts to the current trait environment.

### Adaptable gray colors

class var systemGray: UIColor

The standard base gray color that adapts to the environment.

class var systemGray2: UIColor

A second-level shade of gray that adapts to the environment.

class var systemGray3: UIColor

A third-level shade of gray that adapts to the environment.

class var systemGray4: UIColor

A fourth-level shade of gray that adapts to the environment.

class var systemGray5: UIColor

A fifth-level shade of gray that adapts to the environment.

class var systemGray6: UIColor

A sixth-level shade of gray that adapts to the environment.

### Transparent color

class var clear: UIColor

A color object with grayscale and alpha values that are both `0.0`.

### Fixed colors

class var black: UIColor

A color object in the sRGB color space with a grayscale value of `0.0` and an alpha value of `1.0`.

class var blue: UIColor

A color object with RGB values of `0.0`, `0.0`, and `1.0`, and an alpha value of `1.0`.

class var brown: UIColor

A color object with RGB values of `0.6`, `0.4`, and `0.2`, and an alpha value of `1.0`.

class var cyan: UIColor

A color object with RGB values of `0.0`, `1.0`, and `1.0`, and an alpha value of `1.0`.

class var darkGray: UIColor

A color object with a grayscale value of 1/3 and an alpha value of `1.0`.

class var gray: UIColor

A color object with a grayscale value of `0.5` and an alpha value of `1.0`.

class var green: UIColor

A color object with RGB values of `0.0`, `1.0`, and `0.0`, and an alpha value of `1.0`.

class var lightGray: UIColor

A color object with a grayscale value of 2/3 and an alpha value of `1.0`.

class var magenta: UIColor

A color object with RGB values of `1.0`, `0.0`, and `1.0`, and an alpha value of `1.0`.

class var orange: UIColor

A color object with RGB values of `1.0`, `0.5`, and `0.0`, and an alpha value of `1.0`.

class var purple: UIColor

A color object with RGB values of `0.5`, `0.0`, and `0.5`, and an alpha value of `1.0`.

class var red: UIColor

A color object with RGB values of `1.0`, `0.0`, and `0.0`, and an alpha value of `1.0`.

class var white: UIColor

A color object with a grayscale value of `1.0` and an alpha value of `1.0`.

class var yellow: UIColor

A color object with RGB values of `1.0`, `1.0`, and `0.0`, and an alpha value of `1.0`.

## See Also

### Getting existing colors

UI element colors

Choose colors for UI elements such as labels, text, backgrounds, and links.

Color creation

Load colors from asset catalogs and create colors from raw component values.

