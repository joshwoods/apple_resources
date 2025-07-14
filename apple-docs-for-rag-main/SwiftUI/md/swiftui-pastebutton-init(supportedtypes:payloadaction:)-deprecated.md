

- SwiftUI
- PasteButton
-  init(supportedTypes:payloadAction:) Deprecated

Initializer

# init(supportedTypes:payloadAction:)

Creates a Paste button that accepts specific types of data from the pasteboard.

macOS 10.15–15.4Deprecated

``` source
@MainActor @preconcurrency
init(
    supportedTypes: [String],
    payloadAction: @escaping ([NSItemProvider]) -> Void
)
```

Deprecated

Use the init(supportedContentTypes:payloadAction:) initializer instead.

## Parameters 

`supportedTypes`  

The exact uniform type identifiers supported by the button. If the pasteboard doesn’t contain any of the supported types, the button becomes disabled.

`payloadAction`  

The handler to call when the user clicks the Paste button, and the pasteboard has items that conform to `supportedTypes`. This closure receives an array of item providers that you use to inspect and load the pasteboard data.

## Discussion

Set the contents of `supportedTypes` in order of your app’s preference for its supported types. The Paste button takes the most-preferred type that the pasteboard source supports and delivers this to the `payloadAction` closure.

## See Also

### Deprecated initializers

init&lt;Payload>(supportedTypes: [String], validator: ([NSItemProvider]) -> Payload?, payloadAction: (Payload) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

Deprecated

init&lt;Payload>(supportedContentTypes: [UTType], validator: ([NSItemProvider]) -> Payload?, payloadAction: (Payload) -> Void)

Creates a Paste button that accepts specific types of data from the pasteboard, performing a custom validation of the data before sending it to your app.

Deprecated

