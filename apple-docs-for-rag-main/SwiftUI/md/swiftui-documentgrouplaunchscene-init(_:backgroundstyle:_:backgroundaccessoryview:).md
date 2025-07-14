

- SwiftUI
- DocumentGroupLaunchScene
-  init(\_:backgroundStyle:\_:backgroundAccessoryView:) 

Initializer

# init(\_:backgroundStyle:\_:backgroundAccessoryView:)

Creates a launch scene for document-based applications with a title, a background style, a set of actions, and a background accessory view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
nonisolated
init(
    _ title: LocalizedStringKey,
    backgroundStyle: B = BackgroundStyle(),
    @ViewBuilder _ actions: () -> Actions = { DefaultDocumentGroupLaunchActions() },
    @ViewBuilder backgroundAccessoryView: @escaping (DocumentLaunchGeometryProxy) -> some View
) where B : ShapeStyle
```

Available when `Actions` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A key to use for the view title.

`backgroundStyle`  

A background style of the view.

`actions`  

A view builder for returning the view’s actions.

`backgroundAccessoryView`  

A view builder for returning the view’s background accessory view.

## Discussion

Use a `DocumentGroupLaunchScene` alongside any DocumentGroup scenes. If you don’t implement a `DocumentGroup` in the app declaration, you can get the same design by implementing a DocumentLaunchView.

