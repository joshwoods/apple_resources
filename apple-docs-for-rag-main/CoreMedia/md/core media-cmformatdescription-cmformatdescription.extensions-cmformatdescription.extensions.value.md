

- Core Media
- CMFormatDescription
- CMFormatDescription.Extensions
-  CMFormatDescription.Extensions.Value 

Structure

# CMFormatDescription.Extensions.Value

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Value
```

## Topics

### Extension Values

static func alphaChannelMode(CMFormatDescription.Extensions.Value.AlphaChannelMode) -> CMFormatDescription.Extensions.Value

static func chromaLocation(CMFormatDescription.Extensions.Value.ChromaLocation) -> CMFormatDescription.Extensions.Value

static func cleanAperture(width: (numerator: Int, denominator: Int), height: (numerator: Int, denominator: Int), horizontalOffet: (numerator: Int, denominator: Int), verticalOffset: (numerator: Int, denominator: Int)) -> CMFormatDescription.Extensions.Value

static func cleanAperture&lt;Width, Height, Horizontal, Vertical>(width: Width, height: Height, horizontalOffet: Horizontal, verticalOffset: Vertical) -> CMFormatDescription.Extensions.Value

static func colorPrimaries(CMFormatDescription.Extensions.Value.ColorPrimaries) -> CMFormatDescription.Extensions.Value

static func data(CFData) -> CMFormatDescription.Extensions.Value

static func fieldDetail(CMFormatDescription.Extensions.Value.FieldDetail) -> CMFormatDescription.Extensions.Value

static func fontTable([Int : String]) -> CMFormatDescription.Extensions.Value

static func mobile3GPPTextColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat) -> CMFormatDescription.Extensions.Value

static func mobile3GPPTextDefaultStyle(startChar: Int, endChar: Int, localFontID: Int, fontFace: CMFormatDescription.Extensions.Value.FontFace, fontSize: Int, foregroundColor: CMFormatDescription.Extensions.Value) -> CMFormatDescription.Extensions.Value

static func mpeg2VideoProfile(CMFormatDescription.Extensions.Value.MPEG2VideoProfile) -> CMFormatDescription.Extensions.Value

static func number&lt;T>(T) -> CMFormatDescription.Extensions.Value

static func pixelAspectRatio&lt;Horizontal, Vertical>(horizontalSpacing: Horizontal, verticalSpacing: Vertical) -> CMFormatDescription.Extensions.Value

static func qtTextColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat) -> CMFormatDescription.Extensions.Value

static func qtTextDefaultStyle(startChar: Int, height: Int, ascent: Int, localFontID: Int, fontFace: CMFormatDescription.Extensions.Value.FontFace, fontSize: Int, foregroundColor: CMFormatDescription.Extensions.Value, defaultFontName: String?) -> CMFormatDescription.Extensions.Value

static func sourceReferenceName(value: String, langCode: Int) -> CMFormatDescription.Extensions.Value

static func string(String) -> CMFormatDescription.Extensions.Value

static func string(CFString) -> CMFormatDescription.Extensions.Value

static func textDisplayFlags(Set&lt;CMFormatDescription.Extensions.Value.TextDisplayFlags>) -> CMFormatDescription.Extensions.Value

static func textJustification(CMFormatDescription.Extensions.Value.TextJustification) -> CMFormatDescription.Extensions.Value

static func textRect(top: Int, left: Int, bottom: Int, right: Int) -> CMFormatDescription.Extensions.Value

static func transferFunction(CMFormatDescription.Extensions.Value.TransferFunction) -> CMFormatDescription.Extensions.Value

static func vendor(CMFormatDescription.Extensions.Value.Vendor) -> CMFormatDescription.Extensions.Value

static func vendor(String) -> CMFormatDescription.Extensions.Value

static func yCbCrMatrix(CMFormatDescription.Extensions.Value.YCbCrMatrix) -> CMFormatDescription.Extensions.Value

### Inspecting Extension Values

var propertyListRepresentation: CFPropertyList

### Comparing Extension Values

static func == (CMFormatDescription, CMFormatDescription) -> Bool

Equality is derived from

### Creating Extension Values

init(CFPropertyList)

### Constants

struct AlphaChannelMode

struct ChromaLocation

struct ColorPrimaries

struct FieldDetail

struct FontFace

struct MPEG2VideoProfile

struct TextDisplayFlags

struct TextJustification

struct TransferFunction

struct Vendor

struct YCbCrMatrix

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Constants

struct Key

