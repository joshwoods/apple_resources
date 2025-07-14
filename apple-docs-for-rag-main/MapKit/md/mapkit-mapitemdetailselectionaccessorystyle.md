

- MapKit
-  MapItemDetailSelectionAccessoryStyle 

Structure

# MapItemDetailSelectionAccessoryStyle

The map item detail selection accessory style.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+visionOS 2.0+

``` source
struct MapItemDetailSelectionAccessoryStyle
```

## Topics

### Accessory styles

static var automatic: MapItemDetailSelectionAccessoryStyle

A value that allows the framework to choose an appropriate callout style automatically.

static var callout: MapItemDetailSelectionAccessoryStyle

The accessory, shown as an annotation callout on the map.

static var caption: MapItemDetailSelectionAccessoryStyle

An “Open in Apple Maps” link below the content’s label.

static var sheet: MapItemDetailSelectionAccessoryStyle

The map item detail sheet.

### Callout styles

struct CalloutStyle

The style to use for callout content.

static var automatic: MapItemDetailSelectionAccessoryStyle.CalloutStyle

A value that allows the framework to choose an appropriate callout style automatically.

static var compact: MapItemDetailSelectionAccessoryStyle.CalloutStyle

A compact, space-saving callout style.

static var full: MapItemDetailSelectionAccessoryStyle.CalloutStyle

A rich, detailed callout style that is suitable for large map views.

### Type Methods

static func callout(MapItemDetailSelectionAccessoryStyle.CalloutStyle) -> MapItemDetailSelectionAccessoryStyle

Presents the accessory as an annotation callout on the map.

## See Also

### Place information

func mapItemDetailSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some MapContent

Specifies the selection accessory to display for the selected map item content.

static func callout(MapItemDetailSelectionAccessoryStyle.CalloutStyle) -> MapItemDetailSelectionAccessoryStyle

Presents the accessory as an annotation callout on the map.

