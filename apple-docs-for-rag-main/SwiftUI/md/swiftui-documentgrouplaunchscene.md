

- SwiftUI
-  DocumentGroupLaunchScene 

Structure

# DocumentGroupLaunchScene

A launch scene for document-based applications.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct DocumentGroupLaunchScene where Actions : View
```

## Overview

You can use this launch scene alongside DocumentGroup scenes. If you don’t implement a `DocumentGroup` in the app declaration, you can get the same design by implementing a DocumentLaunchView.

If you don’t provide the title of the scene, it displays the application name. If you don’t provide the actions builder, the scene has the default “Create Document” action that creates new documents. To customize the document launch experience, you can replace the standard screen background and title, add decorative views, and add custom actions.

A `DocumentGroupLaunchScene` configures the document browser on the bottom sheet to open content types from all the document groups in the app definition. A `DocumentGroupLaunchScene` also configures the document groups to create documents of the first content type that your application can create and write.

For more information, see `FileDocument.writableContentTypes` and `ReferenceFileDocument.writableContentTypes`.

## Topics

### Initializers

init(_:_:background:)

Creates a launch scene for document-based applications with a title, a set of actions, and a background.

init(_:_:background:backgroundAccessoryView:)

Creates a launch scene for document-based applications with a title, a set of actions, a background, and a background accessory view.

init(_:_:background:backgroundAccessoryView:overlayAccessoryView:)

Creates a launch scene for document-based applications with a title, a set of actions, and a background.

init(_:_:background:overlayAccessoryView:)

Creates a launch scene for document-based applications with a title, a set of actions, a background, and an overlay accessory view.

init(_:backgroundStyle:_:)

Creates a launch scene for document-based applications with a title, a background style, and a set of actions.

init(_:backgroundStyle:_:backgroundAccessoryView:)

Creates a launch scene for document-based applications with a title, a background style, a set of actions, and a background accessory view.

init(_:backgroundStyle:_:backgroundAccessoryView:overlayAccessoryView:)

Creates a launch scene for document-based applications with a title, a background style, a set of actions, and background and overlay accessory views.

init(_:backgroundStyle:_:overlayAccessoryView:)

Creates a launch scene for document-based applications with a title, a background style, a set of actions, and an overlay accessory view.

## Relationships

### Conforms To

- Scene

## See Also

### Configuring the document launch experience

struct DocumentLaunchView

A view to present when launching document-related user experience.

struct DocumentLaunchGeometryProxy

A proxy for access to the frame of the scene and its title view.

struct DefaultDocumentGroupLaunchActions

The default actions for the document group launch scene and the document launch view.

struct NewDocumentButton

A button that creates and opens new documents.

protocol DocumentBaseBox

A Box that allows setting its Document base not requiring the caller to know the exact types of the box and its base.

