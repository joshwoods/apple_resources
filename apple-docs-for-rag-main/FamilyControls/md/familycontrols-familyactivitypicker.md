

- FamilyControls
-  FamilyActivityPicker 

Structure

# FamilyActivityPicker

A view in which users specify applications, web domains, and categories without revealing their choices to the app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor @preconcurrency
struct FamilyActivityPicker
```

## Overview

To prompt the user for their selection, create a binding to a FamilyActivitySelection instance, and use the binding to create a FamilyActivityPicker instance. You can then display the picker like any SwiftUI view.

```
struct ExampleView: View {
    @State var selection = FamilyActivitySelection()

    var body: some View {
        VStack {
            Image(systemName: "eye")
                .font(.system(size: 76.0))
                .padding()

            FamilyActivityPicker(selection: $selection)

            Image(systemName: "hourglass")
                .font(.system(size: 76.0))
                .padding()
        }
        .onChange(of: selection) { newSelection in
            let applications = selection.applications
            let categories = selection.categories
            let webDomains = selection.webDomains
        }
    }
}
```

Note

A `FamilyControls/FamilyActivityPicker` shown on a parent device only displays applications and websites from authorized child devices within the Family Sharing Group. A `FamilyControls/FamilyActivityPicker` shown on an individually authorized device includes applications and websites from that same device.

To streamline this process, call the familyActivityPicker(isPresented:selection:) modifier on a view in your user interface. This modifier displays the picker view as a sheet over your user interface when the `isPresented` binding is `true`.

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

When you present the `FamilyActivityPicker`, the system displays a view where the user can select categories, applications, and web domains. As soon as the user confirms their selection, the system updates the `FamilyActivitySelection` binding with the user’s selections. To protect the user’s privacy, the system uses opaque values to represent the selections.

Your app passes the selected values to the appropriate instances and methods from the ManagedSettings and DeviceActivity frameworks.

## Topics

### Creating Activity Pickers

init(selection: Binding&lt;FamilyActivitySelection>)

Creates a new activity picker.

func familyActivityPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

### Accessing the Content

var body: some View

The content and behavior of the view.

typealias Body

The type of view representing the body of this view.

### Adding View Modifiers

View Modifiers

Apply standard modifiers to configure the family activity picker view and the views it contains.

### Initializers

init(headerText: String?, footerText: String?, selection: Binding&lt;FamilyActivitySelection>)

Creates a new activity picker with optional header and footer text.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### User-Selected Apps and Web Domains

struct FamilyActivitySelection

A collection of applications, categories, and web domains selected by the user.

