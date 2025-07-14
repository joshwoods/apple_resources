

- SwiftUI
- GroupBox
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a group box with the provided view content and title.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the group box’s title, which describes the content of the group box.

`content`  

A ViewBuilder that produces the content for the group box.

## See Also

### Creating a group box

init(content: () -> Content)

Creates an unlabeled group box with the provided view content.

init(content: () -> Content, label: () -> Label)

Creates a group box with the provided label and view content.

