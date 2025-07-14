

- SwiftUI
- ShareLink
-  init(item:subject:message:) 

Initializer

# init(item:subject:message:)

Creates an instance that presents the share interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    item: String,
    subject: Text? = nil,
    message: Text? = nil
) where Data == CollectionOfOne
```

Available when `Data` conforms to `RandomAccessCollection`, `PreviewImage` is `Never`, `PreviewIcon` is `Never`, `Label` is `DefaultShareLinkLabel`, and `Data.Element` conforms to `Transferable`.

Show all declarations

## Parameters 

`item`  

The item to share.

`subject`  

A title for the item to show when sharing to activities that support a subject field.

`message`  

A description of the item to show when sharing to activities that support a message field. Activities may support attributed text or HTML strings.

## Discussion

Use this initializer when you want the system-standard appearance for `ShareLink`.

## See Also

### Sharing an item

init(_:item:subject:message:)

Creates an instance, with a custom label, that presents the share interface.

init(item:subject:message:label:)

Creates an instance that presents the share interface.

