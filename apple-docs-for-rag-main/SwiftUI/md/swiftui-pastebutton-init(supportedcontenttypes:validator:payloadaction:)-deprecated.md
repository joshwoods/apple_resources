

- SwiftUI
- PasteButton
-  init(supportedContentTypes:validator:payloadAction:) Deprecated

Initializer

# init(supportedContentTypes:validator:payloadAction:)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

macOS 11.0–15.4Deprecated

``` source
@MainActor @preconcurrency
init(
    supportedContentTypes: [UTType],
    validator: @escaping ([NSItemProvider]) -> Payload?,
    payloadAction: @escaping (Payload) -> Void
)
```

Deprecated

Use init(payloadType:onPaste:) instead.

## Parameters 

`supportedContentTypes`  

The exact uniform type identifiers supported by the button. If the pasteboard doesn’t contain any of the supported types, the button becomes disabled.

`validator`  

A handler that receives those contents of the pasteboard that conform to `supportedContentTypes`. Load and inspect these items to determine whether to validate the button. If you load a valid item, return it from this closure. If the pasteboard doesn’t contain any valid items, return `nil` to invalidate the button.

`payloadAction`  

The handler called when the user clicks the button. This closure receives the preprocessed result of `validator`.

## Discussion

Set the contents of `supportedContentTypes` in order of your app’s preference for its supported types. The Paste button takes the most-preferred type that the pasteboard source supports and delivers this to the `validator` closure.

## See Also

### Deprecated initializers

init(supportedTypes: [String], payloadAction: ([NSItemProvider]) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard.

Deprecated

init&lt;Payload>(supportedTypes: [String], validator: ([NSItemProvider]) -> Payload?, payloadAction: (Payload) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

Deprecated

