

- ClockKit
- Deprecated articles and symbols
-  SwiftUI templates 

API Collection

# SwiftUI templates

Design complication templates using SwiftUI views.

## Overview

ClockKit provides SwiftUI versions of the other graphic templates. These templates use a View instance to draw some or all of the complication’s content. However, the following templates are particularly useful when drawing the complication with SwiftUI:

- CLKComplicationTemplateGraphicCircularView

- CLKComplicationTemplateGraphicRectangularFullView

- CLKComplicationTemplateGraphicExtraLargeCircularView

These templates use a single SwiftUI view to fill the entire complication, providing a blank canvas that you can use to draw the entire complication.

## Topics

### Corner templates

class CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

Deprecated

### Circular templates

class CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

### Rectangular templates

class CLKComplicationTemplateGraphicRectangularStandardBodyView

A template for displaying a SwiftUI label and up to three rows of text.

Deprecated

class CLKComplicationTemplateGraphicRectangularTextGaugeView

A template for displaying a header row with a SwiftUI view and text, a second row of text, and a gauge.

Deprecated

class CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

Deprecated

### Extra large templates

class CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

## See Also

### Templates

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

class CLKComplicationTemplate

An abstract class that defines the base behavior for all templates.

Deprecated

enum CLKComplicationFamily

Constants indicating the template groups.

Deprecated

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

Deprecated

