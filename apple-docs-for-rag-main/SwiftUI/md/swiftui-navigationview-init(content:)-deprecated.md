

- SwiftUI
- NavigationView
-  init(content:) Deprecated

Initializer

# init(content:)

Creates a destination-based navigation view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 7.0–11.4Deprecated

``` source
init(@ViewBuilder content: () -> Content)
```

Deprecated

Use NavigationStack and NavigationSplitView instead. For more information, see Migrating to new navigation types.

## Parameters 

`content`  

A ViewBuilder that produces the content that the navigation view wraps. Any views after the first act as placeholders for corresponding columns in a multicolumn display.

## Discussion

Perform navigation by initializing a link with a destination view. For example, consider a `ColorDetail` view that displays a color sample:

```
struct ColorDetail: View {
    var color: Color

    var body: some View {
        color
            .frame(width: 200, height: 200)
            .navigationTitle(color.description.capitalized)
    }
}
```

The following NavigationView presents three links to color detail views:

```
NavigationView {
    List {
        NavigationLink("Purple", destination: ColorDetail(color: .purple))
        NavigationLink("Pink", destination: ColorDetail(color: .pink))
        NavigationLink("Orange", destination: ColorDetail(color: .orange))
    }
    .navigationTitle("Colors")

    Text("Select a Color") // A placeholder to show before selection.
}
```

When the horizontal size class is UserInterfaceSizeClass.regular, like on an iPad in landscape mode, or on a Mac, the navigation view presents itself as a multicolumn view, using its second and later content views — a single Text view in the example above — as a placeholder for the corresponding column:

When the user selects one of the navigation links from the list, the linked destination view replaces the placeholder text in the detail column:

When the size class is UserInterfaceSizeClass.compact, like on an iPhone in portrait orientation, the navigation view presents itself as a single column that the user navigates as a stack. Tapping one of the links replaces the list with the detail view, which provides a back button to return to the list:

