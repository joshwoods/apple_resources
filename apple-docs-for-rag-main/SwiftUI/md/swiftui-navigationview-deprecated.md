

- SwiftUI
-  NavigationView Deprecated

Structure

# NavigationView

A view for presenting a stack of views that represents a visible path in a navigation hierarchy.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 7.0–11.4Deprecated

``` source
struct NavigationView where Content : View
```

Deprecated

Use NavigationStack and NavigationSplitView instead. For more information, see Migrating to new navigation types.

## Mentioned in 

Migrating to new navigation types

Picking container views for your content

Displaying data in lists

## Overview

Use a `NavigationView` to create a navigation-based app in which the user can traverse a collection of views. Users navigate to a destination view by selecting a NavigationLink that you provide. On iPadOS and macOS, the destination content appears in the next column. Other platforms push a new view onto the stack, and enable removing items from the stack with platform-specific controls, like a Back button or a swipe gesture.

Use the init(content:) initializer to create a navigation view that directly associates navigation links and their destination views:

```
NavigationView {
    List(model.notes) { note in
        NavigationLink(note.title, destination: NoteEditor(id: note.id))
    }
    Text("Select a Note")
}
```

Style a navigation view by modifying it with the navigationViewStyle(_:) view modifier. Use other modifiers, like navigationTitle(_:), on views presented by the navigation view to customize the navigation interface for the presented view.

## Topics

### Creating a navigation view

init(content: () -> Content)

Creates a destination-based navigation view.

### Styling navigation views

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

protocol NavigationViewStyle

A specification for the appearance and interaction of a navigation view.

## Relationships

### Conforms To

- View

## See Also

### Deprecated Types

func tabItem&lt;V>(() -> V) -> some View

Sets the tab bar item associated with this view.

Deprecated

