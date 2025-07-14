

- SwiftUI
- View
-  mapFeatureSelectionAccessory(\_:) 

Instance Method

# mapFeatureSelectionAccessory(\_:)

Specifies the selection accessory to display for a `MapFeature`

MapKitSwiftUIiOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func mapFeatureSelectionAccessory(_ style: MapItemDetailSelectionAccessoryStyle? = .automatic) -> some View
```

## Parameters 

`style`  

The map item detail selection accessory style. If `nil`, no selection accessory will be displayed.

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

func mapFeatureSelectionContent(content: (MapFeature) -> some MapContent) -> some View

Specifies a custom presentation for the currently selected feature.

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

