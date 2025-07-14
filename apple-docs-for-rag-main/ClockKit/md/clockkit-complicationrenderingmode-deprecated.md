

- ClockKit
-  ComplicationRenderingMode Deprecated

Enumeration

# ComplicationRenderingMode

The complication’s appearance, as specified by the watch face.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
enum ComplicationRenderingMode
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Building complications with SwiftUI

## Topics

### Rendering Modes

case fullColor

The system renders the complication in full color.

case tinted

The system renders the complication as a tinted complication.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Templates

SwiftUI templates

Design complication templates using SwiftUI views.

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

