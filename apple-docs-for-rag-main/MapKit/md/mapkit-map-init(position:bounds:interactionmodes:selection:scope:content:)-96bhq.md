

- MapKit
- Map
-  init(position:bounds:interactionModes:selection:scope:content:) 

Initializer

# init(position:bounds:interactionModes:selection:scope:content:)

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
init(
    position: Binding,
    bounds: MapCameraBounds? = nil,
    interactionModes: MapInteractionModes = .all,
    selection: Binding,
    scope: Namespace.ID? = nil,
    @MapContentBuilder content: () -> C
) where Content == MapSelectableContentView, SelectedValue : MapSelectable, C : MapContent
```

Available when `Content` conforms to `View`.

