

- SwiftUI
- ShareLink
-  init(item:subject:message:preview:label:) 

Initializer

# init(item:subject:message:preview:label:)

Creates an instance that presents the share interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    item: I,
    subject: Text? = nil,
    message: Text? = nil,
    preview: SharePreview,
    @ViewBuilder label: () -> Label
) where Data == CollectionOfOne, I : Transferable
```

Available when `Data` conforms to `RandomAccessCollection`, `PreviewImage` conforms to `Transferable`, `PreviewIcon` conforms to `Transferable`, `Label` conforms to `View`, and `Data.Element` conforms to `Transferable`.

## Parameters 

`item`  

The item to share.

`subject`  

A title for the item to show when sharing to activities that support a subject field.

`message`  

A description of the item to show when sharing to activities that support a message field. Activities may support attributed text or HTML strings.

`preview`  

A representation of the item to render in a preview.

`label`  

A view builder that produces a label that describes the share action.

## See Also

### Sharing an item with a preview

init&lt;I>(item: I, subject: Text?, message: Text?, preview: SharePreview&lt;PreviewImage, PreviewIcon>)

Creates an instance that presents the share interface.

init(_:item:subject:message:preview:)

Creates an instance, with a custom label, that presents the share interface.

