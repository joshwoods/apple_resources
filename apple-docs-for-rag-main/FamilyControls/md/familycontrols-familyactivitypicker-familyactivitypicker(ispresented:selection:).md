

- FamilyControls
- FamilyActivityPicker
-  familyActivityPicker(isPresented:selection:) 

Instance Method

# familyActivityPicker(isPresented:selection:)

Presents an activity picker view as a sheet.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

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

Use this view modifier to present a FamilyActivityPicker.

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

### Creating Activity Pickers

init(selection: Binding&lt;FamilyActivitySelection>)

Creates a new activity picker.

