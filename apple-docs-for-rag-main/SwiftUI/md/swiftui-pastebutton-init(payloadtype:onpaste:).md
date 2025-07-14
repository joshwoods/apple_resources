

- SwiftUI
- PasteButton
-  init(payloadType:onPaste:) 

Initializer

# init(payloadType:onPaste:)

Creates an instance that accepts values of the specified type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(
    payloadType: T.Type,
    onPaste: @escaping ([T]) -> Void
) where T : Transferable
```

## Parameters 

`onPaste`  

The handler to call on trigger of the button with at least one item of the specified `Transferable` type from the pasteboard.

## See Also

### Creating a paste button

init(supportedContentTypes: [UTType], payloadAction: ([NSItemProvider]) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard.

