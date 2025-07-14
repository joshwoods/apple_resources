

- SwiftUI
- WindowGroup
-  init(\_:for:content:) 

Initializer

# init(\_:for:content:)

Creates a data-presenting window group with a text view title.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
init(
    _ title: Text,
    for type: D.Type,
    @ViewBuilder content: @escaping (Binding) -> C
) where Content == PresentedWindowContent, D : Decodable, D : Encodable, D : Hashable, C : View
```

Available when `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

The Text view to use for the group’s title.

`type`  

The type of presented data this window group accepts.

`content`  

A closure that creates the content for each instance of the group. The closure receives a binding to the value that you pass into the openWindow action when you open the window. SwiftUI automatically persists and restores the value of this binding as part of the state restoration process.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

The system uses the title to distinguish the window group in the user interface, such as in the name of commands associated with the group.

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

SwiftUI creates a window from the group when you present a value of the specified type using the openWindow action.

## See Also

### Creating a data-driven window group

init&lt;D, C>(for: D.Type, content: (Binding&lt;D?>) -> C)

Creates a data-presenting window group.

