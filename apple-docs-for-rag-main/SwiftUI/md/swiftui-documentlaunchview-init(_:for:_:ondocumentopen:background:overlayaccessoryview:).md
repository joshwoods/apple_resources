

- SwiftUI
- DocumentLaunchView
-  init(\_:for:\_:onDocumentOpen:background:overlayAccessoryView:) 

Initializer

# init(\_:for:\_:onDocumentOpen:background:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background view, and an overlay accessory view.

iOS 18.0+iPadOS 18.0+

``` source
init(
    _ title: LocalizedStringKey,
    for contentTypes: [UTType],
    @ViewBuilder _ actions: () -> Actions,
    @ViewBuilder onDocumentOpen: @escaping (URL) -> DocumentView,
    @ViewBuilder background: () -> some View,
    @ViewBuilder overlayAccessoryView: @escaping (DocumentLaunchGeometryProxy) -> some View
)
```

Show all declarations

## Parameters 

`title`  

A title key to use for the view title.

`contentTypes`  

Content types that the view can open.

`actions`  

A view builder returning the view’s actions

`onDocumentOpen`  

A closure that handles an open file.

`background`  

A background of the view.

`overlayAccessoryView`  

A view builder for returning the view’s overlay accessory view.

## Discussion

Note

An alternative to `DocumentLaunchView` is a scene variant of this API: DocumentGroupLaunchScene. If the app definition contains `DocumentGroup` scenes, consider using a `DocumentGroupLaunchScene` instead of this view.

