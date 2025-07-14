

- ClockKit
- Deprecated articles and symbols
-  Graphic 

API Collection

# Graphic

Display visually rich content on watch faces.

## Overview

Use graphic templates to display multicolor text, full-color images, and gauges with color gradients on a variety of watch faces, including the Infograph, Infograph Modular, and Solar Dial.

Note

Watch faces that support graphic templates are available only on Apple Watch Series 4 or later.

ClockKit further divides graphic templates into five different families:

- CLKComplicationFamily.graphicCorner

- CLKComplicationFamily.graphicCircular

- CLKComplicationFamily.graphicBezel

- CLKComplicationFamily.graphicRectangular

- CLKComplicationFamily.graphicExtraLarge.

Each family appears in a different location on the supported watch face. For example, the corner templates can be used in all four corners of the Infographic or Solar Dial watch faces. While the circular templates appear in the center of the Infographic watch face, and along the bottom of the Infographic Modular face.

The graphic families also provide templates that support SwiftUI. These templates use a View instance to draw some or all of the complication’s content. Every graphic template that takes a CLKImageProvider parameter has a variant that takes a View instead.

The CLKComplicationTemplateGraphicRectangularFullView, CLKComplicationTemplateGraphicCircularView, and CLKComplicationTemplateGraphicExtraLargeCircularView provide the most flexibility. In these templates, the SwiftUI view fills the entire complication—giving you a blank canvas that you can use to create your content. For more information, see Building complications with SwiftUI.

### Display Tinted Complications

A watch face that supports graphic complications can display a low-color version of the complication in tinted mode, which makes the following changes to the template:

- Gauges display a solid color instead of a color gradient. The system bases this color on the watch face color the user selected.

- Text displays a color based on the user’s watch face color. Multicolor text providers display only a single color.

- The system automatically desaturates images by default; however, you can use the CLKFullColorImageProvider class’s tintedImageProvider property to provide a tinted version for the image. Note that the complication ignores the tinted image provider’s tintColor property, using a color based on the user’s watch-face color instead.

For more information, see Exploring Tinted Graphic Complications.

## Topics

### Graphic data

Displaying essential information on a watch face

Implement complications in a watch app to display essential information on a watch face.

### Graphic template families

Circular complication templates

Display graphical data in a compact circle.

Corner complication templates

Display graphically rich data in the watch face’s corner.

Rectangular complication templates.

Displays large, rectangular complications for charts, images, or multiple lines of text.

Extra large circular templates

Display large, easy-to-read content on the X-Large watch face.

class CLKComplicationTemplateGraphicBezelCircularText

A template for displaying a circular complication with text along the bezel.

Deprecated

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

class CLKComplicationTemplate

An abstract class that defines the base behavior for all templates.

Deprecated

enum CLKComplicationFamily

Constants indicating the template groups.

Deprecated

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

Deprecated

