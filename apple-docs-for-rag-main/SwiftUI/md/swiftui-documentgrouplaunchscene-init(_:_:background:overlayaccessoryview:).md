

- SwiftUI
- DocumentGroupLaunchScene
-  init(\_:\_:background:overlayAccessoryView:) 

Initializer

# init(\_:\_:background:overlayAccessoryView:)

Creates a launch scene for document-based applications with a title, a set of actions, a background, and an overlay accessory view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
nonisolated
init(
    _ title: LocalizedStringKey,
    @ViewBuilder _ actions: () -> Actions,
    @ViewBuilder background: () -> some View,
    @ViewBuilder overlayAccessoryView: @escaping (DocumentLaunchGeometryProxy) -> some View
)
```

Available when `Actions` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A key to use for the view title.

`actions`  

A view builder for returning the view’s actions.

`background`  

The background of the scene.

`overlayAccessoryView`  

A view builder for returning the view’s overlay accessory view.

## Discussion

Use a `DocumentGroupLaunchScene` alongside any DocumentGroup scenes. If you don’t implement a `DocumentGroup` in the app declaration, you can get the same design by implementing a DocumentLaunchView.

