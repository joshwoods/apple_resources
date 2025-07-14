

- PDFKit
-  PDFAppearanceCharacteristicsKey 

Structure

# PDFAppearanceCharacteristicsKey

Keys to control a widget’s appearance.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAppearanceCharacteristicsKey
```

## Topics

### Modifying Widget Appearance

static let backgroundColor: PDFAppearanceCharacteristicsKey

The background color of the widget annotation.

static let borderColor: PDFAppearanceCharacteristicsKey

The border color of the widget annotation.

static let caption: PDFAppearanceCharacteristicsKey

The text that the button widget annotation displays when the user isn’t interacting with it.

static let downCaption: PDFAppearanceCharacteristicsKey

The text that the button widget annotation displays when the user holds down on it.

static let rolloverCaption: PDFAppearanceCharacteristicsKey

The text that the button widget annotation displays when the user hovers the pointer over it.

static let rotation: PDFAppearanceCharacteristicsKey

The number of degrees, in multiples of 90, that the widget annotation rotates counterclockwise relative to the page.

### Creating an Appearance Characteristic Key

init(rawValue: String)

Creates an appearance characteristic key using the specified raw string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a Widget’s Appearance

var backgroundColor: UIColor?

The background color of the widget annotation.

var borderColor: UIColor?

The border color of the widget annotation.

var caption: String?

The text that the button widget annotation displays when the user isn’t interacting with it.

var controlType: PDFWidgetControlType

The type of button widget annotation.

var downCaption: String?

The text that the button widget annotation displays when the user holds down on it.

var rolloverCaption: String?

The text that the widget annotation displays when the user hovers the pointer over it.

var rotation: Int

The number of degrees, in multiples of 90, that the widget annotation rotates counterclockwise relative to the page.

var appearanceCharacteristicsKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the appearance characteristic key-value pairs.

