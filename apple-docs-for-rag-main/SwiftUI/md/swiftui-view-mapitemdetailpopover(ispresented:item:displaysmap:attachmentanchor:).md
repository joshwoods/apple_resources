

- SwiftUI
- View
-  mapItemDetailPopover(isPresented:item:displaysMap:attachmentAnchor:) 

Instance Method

# mapItemDetailPopover(isPresented:item:displaysMap:attachmentAnchor:)

Presents a map item detail popover.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func mapItemDetailPopover(
    isPresented: Binding,
    item: MKMapItem?,
    displaysMap: Bool = true,
    attachmentAnchor: PopoverAttachmentAnchor = .rect(.bounds)
) -> some View
```

## Parameters 

`isPresented`  

The binding to whether the detail sheet should be shown.

`item`  

The map item to display. If nil, a “loading” view is displayed.

`displaysMap`  

If an inline map should be displayed with the place data. A value of `true` must be specified if the application UI is not already showing the place in a map view.

`attachmentAnchor`  

The positioning anchor that defines the attachment point of the popover. The default is `bounds`.

## Discussion

Use this modifier if you want the system to choose the best orientation of the popover’s arrow. If you want to specify a particular edge for the arrow, use mapItemDetailPopover(isPresented:item:displaysMap:attachmentAnchor:arrowEdge:).

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

func mapItemDetailPopover(isPresented: Binding&lt;Bool>, item: MKMapItem?, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge) -> some View

Presents a map item detail popover.

func mapItemDetailPopover(item: Binding&lt;MKMapItem?>, displaysMap: Bool, attachmentAnchor: PopoverAttachmentAnchor) -> some View

Presents a map item detail popover.

