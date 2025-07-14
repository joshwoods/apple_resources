

- SwiftUI
- PasteButton
-  init(supportedContentTypes:payloadAction:) 

Initializer

# init(supportedContentTypes:payloadAction:)

Creates a Paste button that accepts specific types of data from the pasteboard.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(
    supportedContentTypes: [UTType],
    payloadAction: @escaping ([NSItemProvider]) -> Void
)
```

## Parameters 

`supportedContentTypes`  

The exact uniform type identifiers supported by the button. If the pasteboard doesn’t contain any of the supported types, the button becomes disabled.

`payloadAction`  

The handler to call when the user clicks the Paste button and the pasteboard has items that conform to `supportedContentTypes`. This closure receives an array of item providers that you use to inspect and load the pasteboard data.

## Discussion

Set the contents of `supportedContentTypes` in order of your app’s preference for its supported types. The Paste button takes the most-preferred type that the pasteboard source supports and delivers this to the `payloadAction` closure.

## See Also

### Creating a paste button

init&lt;T>(payloadType: T.Type, onPaste: ([T]) -> Void)

Creates an instance that accepts values of the specified type.

