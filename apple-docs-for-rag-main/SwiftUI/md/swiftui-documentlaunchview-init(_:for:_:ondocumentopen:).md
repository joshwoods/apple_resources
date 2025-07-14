

- SwiftUI
- DocumentLaunchView
-  init(\_:for:\_:onDocumentOpen:) 

Initializer

# init(\_:for:\_:onDocumentOpen:)

Creates a view to present when launching document-related user experiences using a localized title and custom actions.

iOS 18.0+iPadOS 18.0+

``` source
init(
    _ title: LocalizedStringKey,
    for contentTypes: [UTType],
    @ViewBuilder _ actions: () -> Actions,
    @ViewBuilder onDocumentOpen: @escaping (URL) -> DocumentView
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

## Discussion

Note

An alternative to `DocumentLaunchView` is a scene variant of this API: DocumentGroupLaunchScene. If the app definition contains `DocumentGroup` scenes, consider using a `DocumentGroupLaunchScene` instead of this view.

