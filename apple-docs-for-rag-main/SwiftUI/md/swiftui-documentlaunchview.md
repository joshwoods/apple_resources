

- SwiftUI
-  DocumentLaunchView 

Structure

# DocumentLaunchView

A view to present when launching document-related user experience.

iOS 18.0+iPadOS 18.0+

``` source
struct DocumentLaunchView where Actions : View, DocumentView : View
```

## Overview

Note

An alternative to `DocumentLaunchView` is a scene variant of this API: DocumentGroupLaunchScene. If the app definition contains `DocumentGroup` scenes, consider using a `DocumentGroupLaunchScene` instead of this view.

Configure `DocumentLaunchView` to open and display files and trigger custom actions.

For example, an application that offers writing books can present the `DocumentLaunchView` as its launch view:

```
public import UniformTypeIdentifiers

struct BookEditorLaunchView: View {

    var body: some View {
        DocumentLaunchView(for: [.book]) {
            NewDocumentButton("Start New Book")
        } onDocumentOpen: { url in
            BookEditor(url)
        }
    }
}

struct BookEditor: View {
    init(_ url: URL) { }
}

extension UTType {
    static var book = UTType(exportedAs: "com.example.bookEditor")
}
```

## Topics

### Initializers

init(_:for:_:onDocumentOpen:)

Creates a view to present when launching document-related user experiences using a localized title and custom actions.

init(_:for:_:onDocumentOpen:background:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, and a background view.

init(_:for:_:onDocumentOpen:background:backgroundAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background view, and a background accessory view.

init(_:for:_:onDocumentOpen:background:backgroundAccessoryView:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background view, and accessory views.

init(_:for:_:onDocumentOpen:background:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background view, and an overlay accessory view.

init(_:for:_:onDocumentOpen:backgroundAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, and a background accessory view.

init(_:for:_:onDocumentOpen:backgroundAccessoryView:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, and accessory views.

init(_:for:_:onDocumentOpen:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, and an overlay accessory view.

init(_:for:backgroundStyle:_:onDocumentOpen:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, and a background style.

init(_:for:backgroundStyle:_:onDocumentOpen:backgroundAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background style, and a background accessory view.

init(_:for:backgroundStyle:_:onDocumentOpen:backgroundAccessoryView:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background style, and accessory views.

init(_:for:backgroundStyle:_:onDocumentOpen:overlayAccessoryView:)

Creates a view to present when launching document-related user experiences using a localized title, custom actions, a background style, and an overlay accessory view.

### Instance Properties

var body: some View

The body of the view.

## Relationships

### Conforms To

- View

## See Also

### Configuring the document launch experience

struct DocumentGroupLaunchScene

A launch scene for document-based applications.

struct DocumentLaunchGeometryProxy

A proxy for access to the frame of the scene and its title view.

struct DefaultDocumentGroupLaunchActions

The default actions for the document group launch scene and the document launch view.

struct NewDocumentButton

A button that creates and opens new documents.

protocol DocumentBaseBox

A Box that allows setting its Document base not requiring the caller to know the exact types of the box and its base.

