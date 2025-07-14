

- SwiftUI
- WindowGroup
-  init(\_:id:content:) Deprecated

Initializer

# init(\_:id:content:)

Creates a window group with a text view title and an identifier.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    _ title: Text,
    id: String,
    @ViewBuilder content: () -> Content
)
```

Deprecated

Use the initializer which takes an escaping view builder instead.

Show all declarations

## Parameters 

`title`  

The Text view to use for the group’s title.

`id`  

A string that uniquely identifies the window group. Identifiers must be unique among the window groups in your app.

`content`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the specified content as a template to create each window in the group. The system uses the title to distinguish the window group in the user interface, such as in the name of commands associated with the group.

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

## See Also

### Identifying a window group

init(id: String, content: () -> Content)

Creates a window group with an identifier.

Deprecated

