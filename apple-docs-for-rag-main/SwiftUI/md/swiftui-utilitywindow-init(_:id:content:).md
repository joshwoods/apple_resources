

- SwiftUI
- UtilityWindow
-  init(\_:id:content:) 

Initializer

# init(\_:id:content:)

Creates a utility window with a title and identifier.

macOS 15.0+

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

The Text view to use in the utility window’s title bar. Provide a title that describes the purpose of the utility window.

`id`  

An unique string identifier that you can use to open the utility window.

`content`  

The view content to display in the utility window.

## Discussion

Important

The system ignores any text styling that you apply to the Text view title, like bold or italics. However, you can use the formatting controls that the view offers, like for localization, dates, and numerical representations.

