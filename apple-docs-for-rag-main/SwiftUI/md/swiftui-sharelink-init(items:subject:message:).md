

- SwiftUI
- ShareLink
-  init(items:subject:message:) 

Initializer

# init(items:subject:message:)

Creates an instance that presents the share interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    items: Data,
    subject: Text? = nil,
    message: Text? = nil
)
```

Available when `Data` conforms to `RandomAccessCollection`, `PreviewImage` is `Never`, `PreviewIcon` is `Never`, `Label` is `DefaultShareLinkLabel`, and `Data.Element` is `URL`.

Show all declarations

## Parameters 

`items`  

The items to share.

`subject`  

A title for the items to show when sharing to activities that support a subject field.

`message`  

A description of the items to show when sharing to activities that support a message field. Activities may support attributed text or HTML strings.

## Discussion

Use this initializer when you want the system-standard appearance for `ShareLink`.

## See Also

### Sharing items

init(_:items:subject:message:)

Creates an instance, with a custom label, that presents the share interface.

init(items:subject:message:label:)

Creates an instance that presents the share interface.

