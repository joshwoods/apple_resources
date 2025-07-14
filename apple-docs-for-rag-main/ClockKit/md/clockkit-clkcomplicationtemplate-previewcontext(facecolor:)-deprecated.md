

- ClockKit
- CLKComplicationTemplate
-  previewContext(faceColor:) Deprecated

Instance Method

# previewContext(faceColor:)

Returns a view that Xcode can display as a preview.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
func previewContext(faceColor: CLKComplicationTemplate.PreviewFaceColor = .multicolor) -> some View
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`faceColor`  

The tint color for the face. If you omit this parameter, it defaults to a full-color face. For a list of valid face colors, see CLKComplicationTemplate.PreviewFaceColor.

## See Also

### Displaying Previews

struct PreviewFaceColor

The valid face colors for complication templates.

Deprecated

