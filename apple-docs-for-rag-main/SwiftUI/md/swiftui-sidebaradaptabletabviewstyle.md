

- SwiftUI
-  SidebarAdaptableTabViewStyle 

Structure

# SidebarAdaptableTabViewStyle

A tab bar style that adapts to each platform.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct SidebarAdaptableTabViewStyle
```

## Overview

Tab views using the sidebar adaptable style have an appearance that varies depending on the platform:

- iPadOS displays a top tab bar that can adapt into a sidebar.

- iOS displays a bottom tab bar.

- macOS and tvOS always show a sidebar.

- visionOS shows an ornament and also shows a sidebar for secondary tabs within a TabSection.

Use sidebarAdaptable to construct this style.

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

## Topics

### Initializers

init()

## Relationships

### Conforms To

- TabViewStyle

## See Also

### Supporting types

struct DefaultTabViewStyle

The default tab view style.

struct TabBarOnlyTabViewStyle

A tab view style that displays a tab bar when possible.

struct GroupedTabViewStyle

A tab view style that displays a tab bar that groups its tabs together.

struct PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

struct VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical `TabView` interaction and appearance.

struct CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

