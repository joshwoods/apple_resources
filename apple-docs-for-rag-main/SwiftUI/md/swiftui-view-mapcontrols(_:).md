

- SwiftUI
- View
-  mapControls(\_:) 

Instance Method

# mapControls(\_:)

Configures all `Map` views in the associated environment to have standard size and position controls

MapKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func mapControls(@ViewBuilder _ content: () -> some View) -> some View
```

## Parameters 

`content`  

A view builder returning the controls you wish your `Map`

## Discussion

You provide the controls you want to appear atop your map. When using a control in conjunction with `.mapControls` you don’t need to specify a scope. Views that are not MapKit controls will be ignored.

```
Map()
.mapControls {
    MapScaleView()
    MapUserLocationButton()
}
```

Controls can be modified individually or all at once. Custom frames and alignments set on controls are ignored.

```
Map()
.mapControls {
    MapCompass()
        .mapControls(.visible)
    MapPitchToggle()
        .buttonBorderShape(.circular)
        .tint(.purple)
}
.controlSize(.large)
```

On watchOS, space is at a premium. When using the mapControls modifier, MapUserLocationButton and MapCompass are automatically combined if present.

```
Map()
.mapControls {
    MapUserLocationButton()
    MapCompass()
}
```

## See Also

### Getting location information

@MainActor @preconcurrency struct LocationButton

A SwiftUI button that grants one-time location authorization.

@MainActor @preconcurrency struct Map&lt;Content> where Content : View

A view that displays an embedded map interface.

func mapStyle(MapStyle) -> some View

Specifies the map style to be used.

func mapScope(Namespace.ID) -> some View

Creates a mapScope that SwiftUI uses to connect map controls to an associated map.

func mapFeatureSelectionDisabled((MapFeature) -> Bool) -> some View

Specifies which map features should have selection disabled.

func mapFeatureSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some View

Specifies the selection accessory to display for a `MapFeature`

func mapFeatureSelectionContent(content: (MapFeature) -> some MapContent) -> some View

Specifies a custom presentation for the currently selected feature.

func mapControlVisibility(Visibility) -> some View

Configures all Map controls in the environment to have the specified visibility

func mapCameraKeyframeAnimator(trigger: some Equatable, keyframes: (MapCamera) -> some Keyframes&lt;MapCamera>) -> some View

Uses the given keyframes to animate the camera of a `Map` when the given trigger value changes.

func lookAroundViewer(isPresented: Binding&lt;Bool>, scene: Binding&lt;MKLookAroundScene?>, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, onDismiss: (() -> Void)?) -> some View

func lookAroundViewer(isPresented: Binding&lt;Bool>, initialScene: MKLookAroundScene?, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, onDismiss: (() -> Void)?) -> some View

func onMapCameraChange(frequency:_:)

Performs an action when Map camera framing changes

func mapItemDetailPopover(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(item: Binding&lt;MKMapItem?>, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor) -> some View

Presents a map item detail popover.

