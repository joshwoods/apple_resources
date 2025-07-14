

- SwiftUI
- WindowGroup
-  init(\_:content:) Deprecated

Initializer

# init(\_:content:)

Creates a window group with a text view title.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    _ title: Text,
    @ViewBuilder content: () -> Content
)
```

Deprecated

Use the initializer which takes an escaping view builder instead.

Show all declarations

## Parameters 

`title`  

The Text view to use for the group’s title.

`content`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the given view as a template to form the content of each window in the group. The system uses the title to distinguish the window group in the user interface, such as in the name of commands associated with the group.

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

## See Also

### Creating a window group

init(content: () -> Content)

Creates a window group.

Deprecated

