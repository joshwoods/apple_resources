

- ClockKit
-  CLKComplicationTemplateGraphicBezelCircularText Deprecated

Class

# CLKComplicationTemplateGraphicBezelCircularText

A template for displaying a circular complication with text along the bezel.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicBezelCircularText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

The graphic bezel templates display a circular template, and text that wraps around the watch face.

This template belongs to the CLKComplicationFamily.graphicBezel family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The text is optional; this template can either display a circular template with text, or the circular template by itself.

## Topics

### Creating the Template

init(circularTemplate: CLKComplicationTemplateGraphicCircular)

Creates a circular template.

init(circularTemplate: CLKComplicationTemplateGraphicCircular, textProvider: CLKTextProvider?)

Creates a circular template with text that wraps around the bezel.

### Setting the Complication Data

var circularTemplate: CLKComplicationTemplateGraphicCircular

The circular template to display.

var textProvider: CLKTextProvider?

The text to display along the bezel.

## Relationships

### Inherits From

- CLKComplicationTemplate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Graphic template families

Circular complication templates

Display graphical data in a compact circle.

Corner complication templates

Display graphically rich data in the watch face’s corner.

Rectangular complication templates.

Displays large, rectangular complications for charts, images, or multiple lines of text.

Extra large circular templates

Display large, easy-to-read content on the X-Large watch face.

