

- SwiftUI
-  TabSection 

Structure

# TabSection

A container that you can use to add hierarchy within a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TabSection
```

## Overview

Use TabSection to organize tab content into separate sections. Each section has custom tab content that you provide on a per-instance basis. You can also provide a header for each section.

## Topics

### Creating a tab section

init(content:)

Creates a section with the provided section content.

init(_:content:)

Creates a section with the provided content.

init(content:header:)

Creates a section with a header and the provided section content.

### Supporting types

struct DefaultTabLabel

The default label to use for a tab or tab section.

## Relationships

### Conforms To

- Copyable
- TabContent

  Conforms when `Header` conforms to `View`, `Content` conforms to `TabContent`, `Footer` conforms to `View`, and `SelectionValue` is `Content.TabValue`.

## See Also

### Presenting views in tabs

Enhancing your app’s content with tab navigation

Keep your app content front and center while providing quick access to navigation using the tab bar.

struct TabView

A view that switches between multiple child views using interactive user interface elements.

struct Tab

The content for a tab and the tab’s associated tab item in a tab view.

struct TabRole

A value that defines the purpose of the tab.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

