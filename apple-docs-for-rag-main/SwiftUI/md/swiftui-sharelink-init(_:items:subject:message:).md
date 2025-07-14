

- SwiftUI
- ShareLink
-  init(\_:items:subject:message:) 

Initializer

# init(\_:items:subject:message:)

Creates an instance, with a custom label, that presents the share interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ title: Text,
    items: Data,
    subject: Text? = nil,
    message: Text? = nil
)
```

Available when `Data` conforms to `RandomAccessCollection`, `PreviewImage` is `Never`, `PreviewIcon` is `Never`, `Label` is `DefaultShareLinkLabel`, and `Data.Element` is `URL`.

Show all declarations

## Parameters 

`title`  

The title of the share action.

`items`  

The items to share.

`subject`  

A title for the items to show when sharing to activities that support a subject field.

`message`  

A description of the items to show when sharing to activities that support a message field. Activities may support attributed text or HTML strings.

## See Also

### Sharing items

init(items:subject:message:)

Creates an instance that presents the share interface.

init(items:subject:message:label:)

Creates an instance that presents the share interface.

