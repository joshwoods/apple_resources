

- ClockKit
-  CLKComplicationFamily Deprecated

Enumeration

# CLKComplicationFamily

Constants indicating the template groups.

watchOS 2.0+

``` source
enum CLKComplicationFamily
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Topics

### Circular Small

case circularSmall

A small circular area that ClockKit displays on the Color watch face.

### Extra Large

case extraLarge

A large square area that ClockKit displays on the X-Large watch face.

### Modular

case modularSmall

A small square area that ClockKit displays on the Modular watch face.

case modularLarge

A large rectangular area that ClockKit displays on the Modular watch face.

### Utilitarian

case utilitarianSmall

A small square or rectangular area that ClockKit Displays on the Utility, Mickey, Chronograph, and Simple watch faces.

case utilitarianSmallFlat

A small rectangular area that ClockKit Displays on the Photos, Motion, and Timelapse watch faces.

case utilitarianLarge

A large rectangular area that spans the width of the screen in the Utility and Mickey watch faces.

### Graphic

case graphicCorner

A curved area that fills the corners in the Infograph watch face.

case graphicCircular

A circular area that ClockKit displays on the Infograph and Infograph Modular watch faces.

case graphicBezel

A circular area with optional curved text that ClockKit displays along the bezel of the Infograph watch face.

case graphicRectangular

A large rectangular area that ClockKit displays in the center of the Infograph Modular watch face.

case graphicExtraLarge

A large square area that ClockKit displays on the X-Large watch face.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class CLKComplicationTemplate

An abstract class that defines the base behavior for all templates.

Deprecated

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

Deprecated

