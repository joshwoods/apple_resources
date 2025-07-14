

- SwiftUI
-  TabViewStyle 

Protocol

# TabViewStyle

A specification for the appearance and interaction of a tab view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
protocol TabViewStyle
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Getting built-in tab view styles

static var automatic: DefaultTabViewStyle

The default tab view style.

static var carousel: CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

static var page: PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

static func page(indexDisplayMode: PageTabViewStyle.IndexDisplayMode) -> PageTabViewStyle

A `TabViewStyle` that implements a paged scrolling `TabView` with an index display mode.

static var verticalPage: VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical page `TabView` interaction and appearance.

static func verticalPage(transitionStyle: VerticalPageTabViewStyle.TransitionStyle) -> VerticalPageTabViewStyle

A `TabViewStyle` that implements the vertical page `TabView` interaction and appearance, and performs the specified transition.

### Supporting types

struct DefaultTabViewStyle

The default tab view style.

struct SidebarAdaptableTabViewStyle

A tab bar style that adapts to each platform.

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

### Type Properties

static var grouped: GroupedTabViewStyle

A tab view style that displays a tab bar that groups its tabs together.

static var sidebarAdaptable: SidebarAdaptableTabViewStyle

A tab bar style that adapts to each platform.

static var tabBarOnly: TabBarOnlyTabViewStyle

A tab view style that displays a tab bar when possible.

## Relationships

### Conforming Types

- CarouselTabViewStyle
- DefaultTabViewStyle
- GroupedTabViewStyle
- PageTabViewStyle
- SidebarAdaptableTabViewStyle
- TabBarOnlyTabViewStyle
- VerticalPageTabViewStyle

## See Also

### Styling navigation views

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

protocol NavigationSplitViewStyle

A type that specifies the appearance and interaction of navigation split views within a view hierarchy.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

