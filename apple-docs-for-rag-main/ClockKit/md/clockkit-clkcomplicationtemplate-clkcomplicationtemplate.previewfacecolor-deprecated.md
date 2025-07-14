

- ClockKit
- CLKComplicationTemplate
-  CLKComplicationTemplate.PreviewFaceColor Deprecated

Structure

# CLKComplicationTemplate.PreviewFaceColor

The valid face colors for complication templates.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
struct PreviewFaceColor
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Topics

### Colors

static var allColors: [CLKComplicationTemplate.PreviewFaceColor]

An array containing all valid face colors.

static let multicolor: CLKComplicationTemplate.PreviewFaceColor

The preview displays a full-color watch face.

static let pink: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a pink tint color.

static let red: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a red tint color.

static let orange: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with an orange tint color.

static let yellow: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a yellow tint color.

static let green: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a green tint color.

static let blue: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a blue tint color.

static let purple: CLKComplicationTemplate.PreviewFaceColor

The preview displays a watch face with a purple tint color.

## Relationships

### Conforms To

- Identifiable

## See Also

### Displaying Previews

func previewContext(faceColor: CLKComplicationTemplate.PreviewFaceColor) -> some View

Returns a view that Xcode can display as a preview.

Deprecated

