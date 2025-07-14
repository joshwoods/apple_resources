

- ClockKit
- CLKComplicationTemplateGraphicBezelCircularText
-  init(circularTemplate:textProvider:) Deprecated

Initializer

# init(circularTemplate:textProvider:)

Creates a circular template with text that wraps around the bezel.

watchOS 7.0–9.0Deprecated

``` source
init(
    circularTemplate: CLKComplicationTemplateGraphicCircular,
    textProvider: CLKTextProvider?
)
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`circularTemplate`  

A graphic circular template.

`textProvider`  

The text provider for the text element. The template ignores this text provider’s tint color, and always displays the text with a system color.

## See Also

### Creating the Template

init(circularTemplate: CLKComplicationTemplateGraphicCircular)

Creates a circular template.

Deprecated

