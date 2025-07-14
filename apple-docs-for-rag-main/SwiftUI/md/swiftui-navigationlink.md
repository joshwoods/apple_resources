

- SwiftUI
-  NavigationLink 

Structure

# NavigationLink

A view that controls a navigation presentation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct NavigationLink where Label : View, Destination : View
```

## Mentioned in 

Migrating to new navigation types

Displaying data in lists

## Overview

People click or tap a navigation link to present a view inside a NavigationStack or NavigationSplitView. You control the visual appearance of the link by providing view content in the link’s `label` closure. For example, you can use a Label to display a link:

```
NavigationLink {
    FolderDetail(id: workFolder.id)
} label: {
    Label("Work Folder", systemImage: "folder")
}
```

For a link composed only of text, you can use one of the convenience initializers that takes a string and creates a Text view for you:

```
NavigationLink("Work Folder") {
    FolderDetail(id: workFolder.id)
}
```

### Link to a destination view

You can perform navigation by initializing a link with a destination view that you provide in the `destination` closure. For example, consider a `ColorDetail` view that fills itself with a color:

```
struct ColorDetail: View {
    var color: Color

    var body: some View {
        color.navigationTitle(color.description)
    }
}
```

The following NavigationStack presents three links to color detail views:

```
NavigationStack {
    List {
        NavigationLink("Mint") { ColorDetail(color: .mint) }
        NavigationLink("Pink") { ColorDetail(color: .pink) }
        NavigationLink("Teal") { ColorDetail(color: .teal) }
    }
    .navigationTitle("Colors")
}
```

### Create a presentation link

Alternatively, you can use a navigation link to perform navigation based on a presented data value. To support this, use the navigationDestination(for:destination:) view modifier inside a navigation stack to associate a view with a kind of data, and then present a value of that data type from a navigation link. The following example reimplements the previous example as a series of presentation links:

```
NavigationStack {
    List {
        NavigationLink("Mint", value: Color.mint)
        NavigationLink("Pink", value: Color.pink)
        NavigationLink("Teal", value: Color.teal)
    }
    .navigationDestination(for: Color.self) { color in
        ColorDetail(color: color)
    }
    .navigationTitle("Colors")
}
```

Separating the view from the data facilitates programmatic navigation because you can manage navigation state by recording the presented data.

### Control a presentation link programmatically

To navigate programmatically, introduce a state variable that tracks the items on a stack. For example, you can create an array of colors to store the stack state from the previous example, and initialize it as an empty array to start with an empty stack:

```
@State private var colors: [Color] = []
```

Then pass a Binding to the state to the navigation stack:

```
NavigationStack(path: $colors) {
    // ...
}
```

You can use the array to observe the current state of the stack. You can also modify the array to change the contents of the stack. For example, you can programmatically add blue to the array, and navigation to a new color detail view using the following method:

```
func showBlue() {
    colors.append(.blue)
}
```

### Coordinate with a list

You can also use a navigation link to control List selection in a NavigationSplitView:

```
let colors: [Color] = [.mint, .pink, .teal]
@State private var selection: Color? // Nothing selected by default.

var body: some View {
    NavigationSplitView {
        List(colors, id: \.self, selection: $selection) { color in
            NavigationLink(color.description, value: color)
        }
    } detail: {
        if let color = selection {
            ColorDetail(color: color)
        } else {
            Text("Pick a color")
        }
    }
}
```

The list coordinates with the navigation logic so that changing the selection state variable in another part of your code activates the navigation link with the corresponding color. Similarly, if someone chooses the navigation link associated with a particular color, the list updates the selection value that other parts of your code can read.

## Topics

### Presenting a destination view

init(_:destination:)

Creates a navigation link that presents a destination view, with a text label that the link generates from a localized string key.

init(destination:label:)

Creates a navigation link that presents the destination view.

### Presenting a value

init(_:value:)

Creates a navigation link that presents the view corresponding to a codable value, with a text label that the link generates from a localized string key.

init(value:label:)

Creates a navigation link that presents the view corresponding to a codable value.

### Configuring the link

func isDetailLink(Bool) -> some View

Sets the navigation link to present its destination as the detail component of the containing navigation view.

### Deprecated symbols

Deprecated symbols

Review deprecated navigation link initializers.

## Relationships

### Conforms To

- View

## See Also

### Presenting views in columns

Bringing robust navigation structure to your SwiftUI app

Use navigation links, stacks, destinations, and paths to provide a streamlined experience for all platforms, as well as behaviors such as deep linking and state restoration.

Migrating to new navigation types

Improve navigation behavior in your app by replacing navigation views with navigation stacks and navigation split views.

struct NavigationSplitView

A view that presents views in two or three columns, where selections in leading columns control presentations in subsequent columns.

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

struct NavigationSplitViewVisibility

The visibility of the leading columns in a navigation split view.

