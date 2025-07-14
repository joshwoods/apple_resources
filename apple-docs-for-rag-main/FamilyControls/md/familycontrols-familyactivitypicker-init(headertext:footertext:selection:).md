

- FamilyControls
- FamilyActivityPicker
-  init(headerText:footerText:selection:) 

Initializer

# init(headerText:footerText:selection:)

Creates a new activity picker with optional header and footer text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
init(
    headerText: String? = nil,
    footerText: String? = nil,
    selection: Binding
)
```

## Parameters 

`headerText`  

An optional string that provides text for the header of the picker view.

`footerText`  

An optional string that provides text for the footer of the picker view.

`selection`  

A binding that manages the user-selected categories, apps, and web domains.

