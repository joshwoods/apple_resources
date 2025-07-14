

- SwiftUI
-  PasteButton 

Structure

# PasteButton

A system button that reads items from the pasteboard and delivers it to a closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct PasteButton
```

## Overview

Use a paste button when you want to provide a button for pasting items from the system pasteboard into your app. The system provides a button appearance and label appropriate to the current environment. However, you can use view modifiers like buttonBorderShape(_:), labelStyle(_:), and tint(_:) to customize the button in some contexts.

You declare what type of items your app will accept; use a type that conforms to the Transferable protocol. When the user taps or clicks the button, your closure receives the pasteboard items in the specified type.

In the following example, a paste button declares that it accepts a string. When the user taps or clicks the button, the sample’s closure receives an array of strings and sets the first as the value of `pastedText`, which updates a nearby Text view.

```
@State private var pastedText: String = ""

var body: some View {
    HStack {
        PasteButton(payloadType: String.self) { strings in
            pastedText = strings[0]
        }
        Divider()
        Text(pastedText)
        Spacer()
    }
}
```

A paste button automatically validates and invalidates based on changes to the pasteboard on iOS, but not on macOS.

## Topics

### Creating a paste button

init(supportedContentTypes: [UTType], payloadAction: ([NSItemProvider]) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard.

init&lt;T>(payloadType: T.Type, onPaste: ([T]) -> Void)

Creates an instance that accepts values of the specified type.

### Deprecated initializers

init(supportedTypes: [String], payloadAction: ([NSItemProvider]) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard.

Deprecated

init&lt;Payload>(supportedTypes: [String], validator: ([NSItemProvider]) -> Payload?, payloadAction: (Payload) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

Deprecated

init&lt;Payload>(supportedContentTypes: [UTType], validator: ([NSItemProvider]) -> Payload?, payloadAction: (Payload) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

Deprecated

## Relationships

### Conforms To

- View

## See Also

### Creating special-purpose buttons

struct EditButton

A button that toggles the edit mode environment value.

struct RenameButton

A button that triggers a standard rename action.

