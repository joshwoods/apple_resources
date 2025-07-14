

- SwiftUI
-  Tab 

Structure

# Tab

The content for a tab and the tab’s associated tab item in a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Tab
```

## Topics

### Creating a tab

init(content: () -> Content)

Creates a new tab that you can use in a tab view, with an empty label.

init(value:content:)

Creates a new tab that you can use in a tab view, with an empty label.

init(role: TabRole?, content: () -> Content)

Creates a new tab that you can use in a tab view, with an empty label.

init(value:role:content:)

Creates a new tab with a label inferred from the role.

### Creating a tab with label

init(content: () -> Content, label: () -> Label)

Creates a new tab with a label that you can use in a tab view.

### Creating a tab with system symbol

init(_:systemImage:content:)

Creates a new tab that you can use in a tab view using a system image for the tab item’s image, and a localized string key label.

init(_:systemImage:value:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value using a system image for the tab’s tab item image, with a localized string key label.

init(_:systemImage:role:content:)

Creates a new tab that you can use in a tab view using a system image for the tab item’s image, and a localized string key label.

init(_:systemImage:value:role:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value using a system image for the tab’s tab item image, with a localized string key label.

### Creating a tab with image

init(_:image:content:)

Creates a new tab that you can use in a tab view, with a localized string key label.

init(_:image:value:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value, with a localized string key label.

init(_:image:role:content:)

Creates a new tab that you can use in a tab view, with a localized string key label.

init(_:image:value:role:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value, with a localized string key label.

### Supporting types

struct DefaultTabLabel

The default label to use for a tab or tab section.

### Initializers

init(role: TabRole?, content: () -> Content, label: () -> Label)

Creates a new tab with a label that you can use in a tab view.

init(value:content:label:)

Creates a new tab with a label that you can use in a tab view.

init(value:role:content:label:)

Creates a new tab with a label that you can use in a tab view.

## Relationships

### Conforms To

- Copyable
- TabContent

  Conforms when `Value` conforms to `Hashable`, `Content` conforms to `View`, and `Label` conforms to `View`.

## See Also

### Presenting views in tabs

Enhancing your app’s content with tab navigation

Keep your app content front and center while providing quick access to navigation using the tab bar.

struct TabView

A view that switches between multiple child views using interactive user interface elements.

struct TabRole

A value that defines the purpose of the tab.

struct TabSection

A container that you can use to add hierarchy within a tab view.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

