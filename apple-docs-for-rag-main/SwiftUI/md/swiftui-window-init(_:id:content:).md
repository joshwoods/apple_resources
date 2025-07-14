

- SwiftUI
- Window
-  init(\_:id:content:) 

Initializer

# init(\_:id:content:)

Creates a window with a title and an identifier.

macOS 13.0+

``` source
init(
    _ title: Text,
    id: String,
    @ViewBuilder content: () -> Content
)
```

Show all declarations

## Parameters 

`title`  

The Text view to use for the window’s title in system menus and in the window’s title bar. Provide a title that describes the purpose of the window.

`id`  

A unique string identifier that you can use to open the window.

`content`  

The view content to display in the window.

## Discussion

The window displays the view that you specify.

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

