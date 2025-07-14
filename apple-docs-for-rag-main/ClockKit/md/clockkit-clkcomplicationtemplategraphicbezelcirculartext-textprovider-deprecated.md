

- ClockKit
- CLKComplicationTemplateGraphicBezelCircularText
-  textProvider Deprecated

Instance Property

# textProvider

The text to display along the bezel.

watchOS 5.0–9.0Deprecated

``` source
@NSCopying
var textProvider: CLKTextProvider? { get set }
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Discussion

The complication ignores the text provider’s tint color. It always displays the bezel text as white.

## See Also

### Setting the Complication Data

var circularTemplate: CLKComplicationTemplateGraphicCircular

The circular template to display.

Deprecated

