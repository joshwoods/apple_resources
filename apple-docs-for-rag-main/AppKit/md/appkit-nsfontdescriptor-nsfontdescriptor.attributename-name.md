

- AppKit
- NSFontDescriptor
- NSFontDescriptor.AttributeName
-  name 

Type Property

# name

An optional string object that specifies the font name.

macOS

``` source
static let name: NSFontDescriptor.AttributeName
```

## Discussion

The value of this attribute is an NSString object.

## See Also

### Font Attributes

static let family: NSFontDescriptor.AttributeName

An optional string object that specifies the font family.

static let face: NSFontDescriptor.AttributeName

An optional string object that specifies the font face.

static let size: NSFontDescriptor.AttributeName

An optional floating-point number that specifies the font size.

static let visibleName: NSFontDescriptor.AttributeName

An optional string object that specifies the font’s visible name.

static let matrix: NSFontDescriptor.AttributeName

An affine transform that specifies the font’s transformation matrix.

static let variation: NSFontDescriptor.AttributeName

A dictionary that describes the font’s variation axis.

static let characterSet: NSFontDescriptor.AttributeName

The set of Unicode characters covered by the font.

static let cascadeList: NSFontDescriptor.AttributeName

An array, each member of which is a sub-descriptor.

static let traits: NSFontDescriptor.AttributeName

A dictionary that fully describes the font traits.

static let fixedAdvance: NSFontDescriptor.AttributeName

A floating-point value that overrides the glyph advancement specified by the font.

static let featureSettings: NSFontDescriptor.AttributeName

An array of dictionaries representing non-default font feature settings.

