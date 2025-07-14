

- ClockKit
- CLKComplicationTemplateGraphicCornerGaugeImage
-  imageProvider Deprecated

Instance Property

# imageProvider

The image to display.

watchOS 5.0–9.0Deprecated

``` source
@NSCopying
var imageProvider: CLKFullColorImageProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

This image provider produces a full-color image, masked to a circle.

## See Also

### Setting the Complication Data

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

Deprecated

var leadingTextProvider: CLKTextProvider?

The text to display on the leading edge of the gauge.

Deprecated

var trailingTextProvider: CLKTextProvider?

The text to display on the trailing edge of the gauge.

Deprecated

