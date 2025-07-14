

- SwiftUI
- WindowGroup
-  init(\_:makeContent:) 

Initializer

# init(\_:makeContent:)

Creates a window group with a text view title.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ title: Text,
    @ViewBuilder makeContent: @escaping () -> Content
)
```

Available when `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

The Text view to use for the group’s title.

`makeContent`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the given view as a template to form the content of each window in the group. The system uses the title to distinguish the window group in the user interface, such as in the name of commands associated with the group.

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

