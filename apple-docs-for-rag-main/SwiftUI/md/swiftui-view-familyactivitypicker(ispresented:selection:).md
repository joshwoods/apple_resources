

- SwiftUI
- View
-  familyActivityPicker(isPresented:selection:) 

Instance Method

# familyActivityPicker(isPresented:selection:)

Presents an activity picker view as a sheet.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor @preconcurrency
func familyActivityPicker(
    isPresented: Binding,
    selection: Binding
) -> some View
```

## Parameters 

`isPresented`  

A binding that indicates whether the app presents the picker view.

`selection`  

A binding that manages the user-selected categories, apps, and web domains.

## Discussion

Use this view modifier to present a `FamilyControls/FamilyActivityPicker`.

```
struct ExampleView: View {
    @State var selection = FamilyActivitySelection()
    @State var isPresented = false

   var body: some View {
       Button("Present FamilyActivityPicker") { isPresented = true }
       .familyActivityPicker(isPresented: $isPresented,
                             selection: $selection)
       .onChange(of: selection) { newSelection in
           let applications = selection.applications
           let categories = selection.categories
           let webDomains = selection.webDomains
       }
   }
}
```

## See Also

### Configuring Family Sharing

@MainActor @preconcurrency struct FamilyActivityPicker

A view in which users specify applications, web domains, and categories without revealing their choices to the app.

func familyActivityPicker(headerText: String?, footerText: String?, isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

