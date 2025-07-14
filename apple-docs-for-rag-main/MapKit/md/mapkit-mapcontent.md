

- MapKit
-  MapContent 

Protocol

# MapContent

A protocol used to construct map content such as controls, markers, and annotations.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
protocol MapContent
```

## Topics

### Accessing the view body

var body: Self.Body

The content and behavior of the view.

**Required**

### Supplying annotation titles

func annotationTitles(Visibility) -> some MapContent

Sets the visibility of titles for markers and annotations.

func annotationSubtitles(Visibility) -> some MapContent

Sets the visibility of subtitles for markers and annotations.

### Setting the content style

func foregroundStyle(some ShapeStyle) -> some MapContent

Specifies the shape style used to fill content in drawing map overlays.

func tint&lt;S>(S) -> some MapContent

The tint shape style to apply to map content.

### Setting stroke properties

func stroke(some ShapeStyle, lineWidth: CGFloat) -> some MapContent

Applies the given shape style to drawn map overlays using the line width you specify.

func stroke(some ShapeStyle, style: StrokeStyle) -> some MapContent

Applies the given shape style to drawn map overlays using the stroke style you specify.

func stroke(lineWidth: CGFloat) -> some MapContent

Applies the given stoke drawn map overlays using the line width you specify.

func strokeStyle(style: StrokeStyle) -> some MapContent

Applies the given stroke style to drawn map overlays.

### Setting the overlay level

func mapOverlayLevel(level: MKOverlayLevel) -> some MapContent

Specifies the position of overlays relative to other map content.

### Associated types

associatedtype Body : MapContent

The content and behavior of the view.

**Required**

### Displaying place information

func mapItemDetailSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some MapContent

Specifies the selection accessory to display for the selected map item content.

### Instance Methods

func tag&lt;V>(V) -> some MapContent

Sets the unique tag value of this piece of map content.

## Relationships

### Inherited By

- DynamicMapContent

### Conforming Types

- Annotation
- AnyMapContent
- EmptyMapContent
- MapCircle
- MapPolygon
- MapPolyline
- Marker
- TupleMapContent
- UserAnnotation

## See Also

### Protocols

protocol DynamicMapContent

A  type of view that generates views from an underlying collection of data.

struct MapContentBuilder

A result builder that creates map content from closures you provide.

struct MapContentView

A view that contains content that displays on a map at a specific position, and that responds to specific interactions you specify.

