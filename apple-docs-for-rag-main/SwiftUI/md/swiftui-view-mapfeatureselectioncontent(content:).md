

- SwiftUI
- View
-  mapFeatureSelectionContent(content:) 

Instance Method

# mapFeatureSelectionContent(content:)

Specifies a custom presentation for the currently selected feature.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor @preconcurrency
func mapFeatureSelectionContent(@MapContentBuilder content: @escaping (MapFeature) -> some MapContent) -> some View
```

## Parameters 

`content`  

Generates the custom presentation for a given map feature.

## Discussion

The supported presentation options are `Annotation`, and `Marker`. Other types of map content will be ignored and handled as though no content was returned.

If empty map content is returned, the system presentation will be used.

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

func mapControls(() -> some View) -> some View

Configures all `Map` views in the associated environment to have standard size and position controls

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

