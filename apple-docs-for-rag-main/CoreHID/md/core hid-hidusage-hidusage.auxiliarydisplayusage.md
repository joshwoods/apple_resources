

- Core HID
- HIDUsage
-  HIDUsage.AuxiliaryDisplayUsage 

Enumeration

# HIDUsage.AuxiliaryDisplayUsage

macOS 15.0+

``` source
enum AuxiliaryDisplayUsage
```

## Topics

### Enumeration Cases

case alphanumericDisplay

case asciiCharacterSet

case attributeData

case attributeReadback

case auxiliaryDisplay

case bitDepthFormat

case bitmapSizeX

case bitmapSizeY

case blitData

case blitRectangleX1

case blitRectangleX2

case blitRectangleY1

case blitRectangleY2

case blitReport

case charAttrBlink

case charAttrEnhance

case charAttrUnderline

case characterAttribute

case characterHeight

case characterMapping

case characterPageMapping

case characterReport

case characterSpacingHorizontal

case characterSpacingVertical

case characterWidth

case clearDisplay

case column

case columns

case cursorBlink

case cursorEnable

case cursorMode

case cursorPixelPositioning

case cursorPositionReport

case dataReadBack

case displayAttributesReport

case displayBrightness

case displayContrast

case displayControlReport

case displayData

case displayDataExtensions

case displayEnable

case displayOrientation

case displayStatus

case errorFontDataCannotBeRead

case errorNotALoadableCharacter

case font14Segment

case font7Segment

case fontData

case fontReadBack

case fontReport

case fourteenSegmentDirectMap

case horizontalScroll

case maxBlitSize

case paletteData

case paletteDataOffset

case paletteDataSize

case paletteReport

case requestReport

case row

case rows

case screenSaverDelay

case screenSaverEnable

case sevenSegmentDirectMap

case softButton

case softButtonID

case softButtonOffset1

case softButtonOffset2

case softButtonReport

case softButtonSide

case softKeys

case statNotReady

case statReady

case unicodeCharacterSet

case unicodeEquivalent

case verticalScroll

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

