

- ClockKit
-  CLKComplicationTemplate Deprecated

Class

# CLKComplicationTemplate

An abstract class that defines the base behavior for all templates.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplate
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

You don’t create instances of this class directly. Instead, you create instances of one of the concrete subclasses and use the resulting object to specify the data for your complication.

## Topics

### Setting the Tint Color

var tintColor: UIColor?

The tint color to apply to elements of the template.

### Displaying Previews

func previewContext(faceColor: CLKComplicationTemplate.PreviewFaceColor) -> some View

Returns a view that Xcode can display as a preview.

struct PreviewFaceColor

The valid face colors for complication templates.

### Specifying Styles

enum CLKComplicationColumnAlignment

Constants indicating the alignment of text in columns.

enum CLKComplicationRingStyle

Constants indicating the appearance of a progress ring.

### Creating Empty Templates

init()

Creates a new complication.

class func new() -> Self

Returns a new complication.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLKComplicationTemplateCircularSmallRingImage
- CLKComplicationTemplateCircularSmallRingText
- CLKComplicationTemplateCircularSmallSimpleImage
- CLKComplicationTemplateCircularSmallSimpleText
- CLKComplicationTemplateCircularSmallStackImage
- CLKComplicationTemplateCircularSmallStackText
- CLKComplicationTemplateExtraLargeColumnsText
- CLKComplicationTemplateExtraLargeRingImage
- CLKComplicationTemplateExtraLargeRingText
- CLKComplicationTemplateExtraLargeSimpleImage
- CLKComplicationTemplateExtraLargeSimpleText
- CLKComplicationTemplateExtraLargeStackImage
- CLKComplicationTemplateExtraLargeStackText
- CLKComplicationTemplateGraphicBezelCircularText
- CLKComplicationTemplateGraphicCircular
- CLKComplicationTemplateGraphicCornerCircularImage
- CLKComplicationTemplateGraphicCornerCircularView
- CLKComplicationTemplateGraphicCornerGaugeImage
- CLKComplicationTemplateGraphicCornerGaugeText
- CLKComplicationTemplateGraphicCornerGaugeView
- CLKComplicationTemplateGraphicCornerStackText
- CLKComplicationTemplateGraphicCornerTextImage
- CLKComplicationTemplateGraphicCornerTextView
- CLKComplicationTemplateGraphicExtraLargeCircular
- CLKComplicationTemplateGraphicRectangularFullImage
- CLKComplicationTemplateGraphicRectangularFullView
- CLKComplicationTemplateGraphicRectangularLargeImage
- CLKComplicationTemplateGraphicRectangularLargeView
- CLKComplicationTemplateGraphicRectangularStandardBody
- CLKComplicationTemplateGraphicRectangularStandardBodyView
- CLKComplicationTemplateGraphicRectangularTextGauge
- CLKComplicationTemplateGraphicRectangularTextGaugeView
- CLKComplicationTemplateModularLargeColumns
- CLKComplicationTemplateModularLargeStandardBody
- CLKComplicationTemplateModularLargeTable
- CLKComplicationTemplateModularLargeTallBody
- CLKComplicationTemplateModularSmallColumnsText
- CLKComplicationTemplateModularSmallRingImage
- CLKComplicationTemplateModularSmallRingText
- CLKComplicationTemplateModularSmallSimpleImage
- CLKComplicationTemplateModularSmallSimpleText
- CLKComplicationTemplateModularSmallStackImage
- CLKComplicationTemplateModularSmallStackText
- CLKComplicationTemplateUtilitarianLargeFlat
- CLKComplicationTemplateUtilitarianSmallFlat
- CLKComplicationTemplateUtilitarianSmallRingImage
- CLKComplicationTemplateUtilitarianSmallRingText
- CLKComplicationTemplateUtilitarianSmallSquare

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Templates

SwiftUI templates

Design complication templates using SwiftUI views.

enum ComplicationRenderingMode

The complication’s appearance, as specified by the watch face.

Deprecated

Data providers

Feed data to a complication template.

Circular small

Display small, circular content in the corners of the Color watch face.

Extra large

Display content on the X-Large watch face.

Modular small

Display content in the smaller spaces of the Modular watch face.

Modular large

Display multiple rows of content in the large, central complication on the Modular watch face.

Utilitarian

Use the utilitarian templates to display content on a variety of watch faces, including the Utility, Chronograph, Simple, and character watch faces.

Graphic

Display visually rich content on watch faces.

enum CLKComplicationFamily

Constants indicating the template groups.

Deprecated

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

Deprecated

