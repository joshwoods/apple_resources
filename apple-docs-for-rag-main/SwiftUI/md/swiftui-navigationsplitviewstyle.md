

- SwiftUI
-  NavigationSplitViewStyle 

Protocol

# NavigationSplitViewStyle

A type that specifies the appearance and interaction of navigation split views within a view hierarchy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol NavigationSplitViewStyle
```

## Overview

To configure the navigation split view style for a view hierarchy, use the navigationSplitViewStyle(_:) modifier.

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

### Creating built-in styles

static var automatic: AutomaticNavigationSplitViewStyle

A navigation split style that resolves its appearance automatically based on the current context.

static var balanced: BalancedNavigationSplitViewStyle

A navigation split style that reduces the size of the detail content to make room when showing the leading column or columns.

static var prominentDetail: ProminentDetailNavigationSplitViewStyle

A navigation split style that attempts to maintain the size of the detail content when hiding or showing the leading columns.

### Creating custom styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a navigation split view.

**Required**

typealias Configuration

The properties of a navigation split view instance.

associatedtype Body : View

A view that represents the body of a navigation split view.

**Required**

### Supporting types

struct AutomaticNavigationSplitViewStyle

A navigation split style that resolves its appearance automatically based on the current context.

struct BalancedNavigationSplitViewStyle

A navigation split style that reduces the size of the detail content to make room when showing the leading column or columns.

struct ProminentDetailNavigationSplitViewStyle

A navigation split style that attempts to maintain the size of the detail content when hiding or showing the leading columns.

struct NavigationSplitViewStyleConfiguration

The properties of a navigation split view instance.

## Relationships

### Conforming Types

- AutomaticNavigationSplitViewStyle
- BalancedNavigationSplitViewStyle
- ProminentDetailNavigationSplitViewStyle

## See Also

### Styling navigation views

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

protocol TabViewStyle

A specification for the appearance and interaction of a tab view.

