

- SwiftUI
- ShareLink
-  init(items:subject:message:preview:) 

Initializer

# init(items:subject:message:preview:)

Creates an instance that presents the share interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    items: Data,
    subject: Text? = nil,
    message: Text? = nil,
    preview: @escaping (Data.Element) -> SharePreview
)
```

Available when `Data` conforms to `RandomAccessCollection`, `PreviewImage` conforms to `Transferable`, `PreviewIcon` conforms to `Transferable`, `Label` is `DefaultShareLinkLabel`, and `Data.Element` conforms to `Transferable`.

## Parameters 

`items`  

The items to share.

`subject`  

A title for the items to show when sharing to activities that support a subject field.

`message`  

A description of the items to show when sharing to activities that support a message field. Activities may support attributed text or HTML strings.

`preview`  

A closure that returns a representation of each item to render in a preview.

## Discussion

Use this initializer when you want the system-standard appearance for `ShareLink`.

## See Also

### Sharing items with a preview

init(_:items:subject:message:preview:)

Creates an instance, with a custom label, that presents the share interface.

init(items: Data, subject: Text?, message: Text?, preview: (Data.Element) -> SharePreview&lt;PreviewImage, PreviewIcon>, label: () -> Label)

Creates an instance that presents the share interface.

