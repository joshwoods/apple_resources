

- PDFKit
- PDFAppearanceCharacteristics
-  downCaption 

Instance Property

# downCaption

The text that the button widget annotation displays when the user holds down on it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var downCaption: String? { get set }
```

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

var rolloverCaption: String?

The text that the widget annotation displays when the user hovers the pointer over it.

var rotation: Int

The number of degrees, in multiples of 90, that the widget annotation rotates counterclockwise relative to the page.

var appearanceCharacteristicsKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the appearance characteristic key-value pairs.

struct PDFAppearanceCharacteristicsKey

Keys to control a widget’s appearance.

