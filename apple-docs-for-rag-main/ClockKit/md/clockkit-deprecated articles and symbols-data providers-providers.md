

- ClockKit
- Deprecated articles and symbols
-  Data providers 

API Collection

# Data providers

Feed data to a complication template.

## Topics

### Text providers

class CLKSimpleTextProvider

A single line of text to display in your complication interface.

Deprecated

class CLKDateTextProvider

A formatted string that conveys a date without any time information.

Deprecated

class CLKRelativeDateTextProvider

A formatted string that conveys the difference in time between the current date and a date that you specify.

Deprecated

class CLKTimeIntervalTextProvider

A formatted time range.

Deprecated

class CLKTimeTextProvider

A formatted time value.

Deprecated

class CLKTextProvider

The common behavior for displaying text-based data in a complication.

Deprecated

### Image providers

class CLKImageProvider

An image displayed by a complication.

Deprecated

class CLKFullColorImageProvider

A full-color image displayed by a complication.

Deprecated

### Gauge providers

class CLKSimpleGaugeProvider

A gauge that shows a fractional value.

Deprecated

class CLKTimeIntervalGaugeProvider

A gauge that tracks time intervals.

Deprecated

class CLKGaugeProvider

An abstract superclass that provides all the common behaviors for the gauge providers.

Deprecated

let CLKSimpleGaugeProviderFillFractionEmpty: Float

A fill value indicating an empty gauge.

Deprecated

enum CLKGaugeProviderStyle

Visual styles available for gauges.

Deprecated

## See Also

### Templates

SwiftUI templates

Design complication templates using SwiftUI views.

enum ComplicationRenderingMode

The complication’s appearance, as specified by the watch face.

Deprecated

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

