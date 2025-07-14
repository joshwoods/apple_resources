

- SwiftUI
- View
-  familyActivityPicker(headerText:footerText:isPresented:selection:) 

Instance Method

# familyActivityPicker(headerText:footerText:isPresented:selection:)

Presents an activity picker view as a sheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
func familyActivityPicker(
    headerText: String? = nil,
    footerText: String? = nil,
    isPresented: Binding,
    selection: Binding
) -> some View
```

## Parameters 

`headerText`  

An optional string that provides text for the header of the picker view.

`footerText`  

An optional string that provides text for the footer of the picker view.

`isPresented`  

A binding that indicates whether the app presents the picker view.

`selection`  

A binding that manages the user-selected categories, apps, and web domains.

## Discussion

Use this view modifier to present a `FamilyControls/FamilyActivityPicker`.

## See Also

### Configuring Family Sharing

@MainActor @preconcurrency struct FamilyActivityPicker

A view in which users specify applications, web domains, and categories without revealing their choices to the app.

func familyActivityPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

