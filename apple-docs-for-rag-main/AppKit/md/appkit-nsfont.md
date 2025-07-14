

- AppKit
-  NSFont 

Class

# NSFont

The representation of a font in an app.

macOS

``` source
class NSFont
```

## Overview

NSFont objects represent fonts to an app, providing access to characteristics of the font and assistance in laying out glyphs relative to one another. Font objects are also used to establish the current font for drawing text directly into a graphics context, using the set() method.

You don’t create NSFont objects using the `alloc` and `init` methods. Instead, you use either init(descriptor:size:) or init(name:size:) to look up an available font and alter its size or matrix to your needs. These methods check for an existing font object with the specified characteristics, returning it if there is one. Otherwise, they look up the font data requested and create the appropriate object. NSFont also defines a number of methods for getting standard system fonts, such as systemFont(ofSize:), userFont(ofSize:), and messageFont(ofSize:). To request the default size for these standard fonts, pass a negative number or `0` as the font size. See macOS Human Interface Guidelines for more information about system fonts.

## Topics

### Creating Arbitrary Fonts

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

init?(descriptor: NSFontDescriptor, size: CGFloat)

Returns a font object for the specified font descriptor and font size.

init?(descriptor: NSFontDescriptor, textTransform: AffineTransform?)

Returns a font object for the specified font descriptor and text transform.

init?(name: String, matrix: UnsafePointer&lt;CGFloat>)

Returns a font object for the specified font name and matrix.

### Creating User Fonts

class func userFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), in the specified size.

class func userFixedPitchFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), when that font should be fixed-pitch, in the specified size.

### Creating System Fonts

class func preferredFont(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFont

Returns the font associated with the text style.

class func systemFont(ofSize: CGFloat) -> NSFont

Returns the standard system font with the specified size.

class func systemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns the standard system font with the specified size and weight.

class func boldSystemFont(ofSize: CGFloat) -> NSFont

Returns the standard system font in boldface type with the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns a monospace version of the system font with the specified size and weight.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns a version of the standard system font that contains monospaced digit glyphs.

class var systemFontSize: CGFloat

Returns the size of the standard system font.

class var smallSystemFontSize: CGFloat

Returns the size of the standard small system font.

struct Weight

System-defined font-weight values.

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

struct TextStyleOptionKey

The options that you apply when requesting the font or font descriptor of a preferred text style.

### Creating UI Element Fonts

class func labelFont(ofSize: CGFloat) -> NSFont

Returns the font used for standard interface labels in the specified size.

class func messageFont(ofSize: CGFloat) -> NSFont

Returns the font used for standard interface items, such as button labels, menu items, and so on, in the specified size.

class func menuBarFont(ofSize: CGFloat) -> NSFont

Returns the font used for menu bar items, in the specified size.

class func menuFont(ofSize: CGFloat) -> NSFont

Returns the font used for menu items, in the specified size.

class func controlContentFont(ofSize: CGFloat) -> NSFont

Returns the font used for the content of controls in the specified size.

class func titleBarFont(ofSize: CGFloat) -> NSFont

Returns the font used for window title bars, in the specified size.

class func paletteFont(ofSize: CGFloat) -> NSFont

Returns the font used for palette window title bars, in the specified size.

class func toolTipsFont(ofSize: CGFloat) -> NSFont

Returns the font used for tool tips labels, in the specified size.

class var labelFontSize: CGFloat

Returns the size of the standard label font.

class func systemFontSize(for: NSControl.ControlSize) -> CGFloat

Returns the font size used for the specified control size.

### Using a Font to Draw

func set()

Sets this font as the font for the current graphics context.

func set(in: NSGraphicsContext)

Sets this font as the font for the specified graphics context.

### Getting Font Metrics and Information

var pointSize: CGFloat

The point size of the font.

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var fontDescriptor: NSFontDescriptor

The font descriptor object for the font.

var isFixedPitch: Bool

A Boolean value indicating whether all glyphs in the font have the same advancement.

var mostCompatibleStringEncoding: UInt

The string encoding that works best with the font.

Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

### Getting Information About Glyphs

var numberOfGlyphs: Int

The number of glyphs in the font.

typealias NSGlyph

The type used to specify glyphs.

var NSControlGlyph: Int

The reserved code for a control glyph.

var NSNullGlyph: Int

The reserved code for a null glyph.

### Getting Font Names

var displayName: String?

The name of the font, including family and face names, to use when displaying the font information to the user.

var familyName: String?

The family name of the font—for example, “Times” or “Helvetica.”

var fontName: String

The full name of the font, as used in PostScript language code—for example, “Times-Roman” or “Helvetica-Oblique.”

### Setting User Fonts

class func setUser(NSFont?)

Sets the font used by default for documents and other text under the user’s control to the specified font.

class func setUserFixedPitch(NSFont?)

Sets the font used by default for documents and other text under the user’s control, when that font should be fixed-pitch, to the specified font.

### Vertical Fonts

var isVertical: Bool

A Boolean value indicating whether the font is a vertical font.

var vertical: NSFont

A vertical version of the font.

### Responding to Font-Related Notifications

class let antialiasThresholdChangedNotification: NSNotification.Name

Posted after the threshold for antialiasing changes.

class let fontSetChangedNotification: NSNotification.Name

Posted after the currently-set font changes.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

### Type Aliases

struct Width

### Instance Properties

var printer: NSFont

The scalable PostScript font corresponding to current font.

var renderingMode: NSFontRenderingMode

The rendering mode of the font.

var screen: NSFont

The bitmapped screen font for the current font.

### Instance Methods

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

func boundingRect(forGlyph: NSGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

Deprecated

func getAdvancements(NSSizeArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

Deprecated

func getAdvancements(NSSizeArray, forPackedGlyphs: UnsafeRawPointer, length: Int)

Returns an array of the advancements for the specified packed glyphs and rendered by the receiver.

Deprecated

func getBoundingRects(NSRectArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

Deprecated

func glyph(withName: String) -> NSGlyph

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

func withSize(CGFloat) -> NSFont

### Type Methods

class func systemFont(ofSize: CGFloat, weight: NSFont.Weight, width: NSFont.Width) -> NSFont

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Font Data

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

