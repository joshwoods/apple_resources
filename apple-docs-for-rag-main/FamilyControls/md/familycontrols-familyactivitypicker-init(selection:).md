

- FamilyControls
- FamilyActivityPicker
-  init(selection:) 

Initializer

# init(selection:)

Creates a new activity picker.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor @preconcurrency
init(selection: Binding)
```

## Parameters 

`selection`  

A binding that manages the user-selected categories, apps, and web domains.

## See Also

### Creating Activity Pickers

func familyActivityPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

