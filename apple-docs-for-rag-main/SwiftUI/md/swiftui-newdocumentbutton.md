

- SwiftUI
-  NewDocumentButton 

Structure

# NewDocumentButton

A button that creates and opens new documents.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct NewDocumentButton where Label : View
```

## Overview

Use a new document button to give people the option to create documents in your app. In the following example, there are two new document buttons, both support Text labels. When the user taps or clicks the first button, the system creates a new document in the directory currently open in the document browser. The second button creates a new document from a template.

```
@State private var isTemplatePickerPresented = false
@State private var documentCreationContinuation:
    CheckedContinuation?

var body: some Scene {
    DocumentGroupLaunchScene("My Documents") {
        NewDocumentButton("Start Writing…")
        NewDocumentButton("Choose a Template", for: MyDocument.self) {
            try await withCheckedThrowingContinuation { continuation in
                documentCreationContinuation = continuation
                isTemplatePickerPresented = true
            }
        }
        .fullScreenCover(isPresented: $isTemplatePickerPresented) {
            TemplatePicker(continuation: $documentCreationContinuation)
        }
    }
}
```

If you don’t provide a custom label, the system provides a button with the default “Create Document” label.

## Topics

### Initializers

init(_:contentType:)

Creates and opens new documents.

init(_:contentType:prepareDocumentURL:)

Creates and opens new documents.

init(_:for:contentType:prepareDocument:)

Creates and opens new documents.

## Relationships

### Conforms To

- View

## See Also

### Configuring the document launch experience

struct DocumentGroupLaunchScene

A launch scene for document-based applications.

struct DocumentLaunchView

A view to present when launching document-related user experience.

struct DocumentLaunchGeometryProxy

A proxy for access to the frame of the scene and its title view.

struct DefaultDocumentGroupLaunchActions

The default actions for the document group launch scene and the document launch view.

protocol DocumentBaseBox

A Box that allows setting its Document base not requiring the caller to know the exact types of the box and its base.

