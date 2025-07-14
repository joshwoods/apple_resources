

- MapKit
- MapContent
-  mapItemDetailSelectionAccessory(\_:) 

Instance Method

# mapItemDetailSelectionAccessory(\_:)

Specifies the selection accessory to display for the selected map item content.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func mapItemDetailSelectionAccessory(_ style: MapItemDetailSelectionAccessoryStyle? = .automatic) -> some MapContent
```

## Parameters 

`style`  

The map item detail selection accessory style. If `nil`, no selection accessory appears.

## See Also

### Place information

struct MapItemDetailSelectionAccessoryStyle

The map item detail selection accessory style.

static func callout(MapItemDetailSelectionAccessoryStyle.CalloutStyle) -> MapItemDetailSelectionAccessoryStyle

Presents the accessory as an annotation callout on the map.

