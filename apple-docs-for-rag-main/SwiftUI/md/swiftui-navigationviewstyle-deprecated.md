

- SwiftUI
-  NavigationViewStyle Deprecated

Protocol

# NavigationViewStyle

A specification for the appearance and interaction of a navigation view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 7.0–11.4Deprecated

``` source
protocol NavigationViewStyle
```

Deprecated

Replace a styled NavigationView with a NavigationStack or NavigationSplitView. For more information, see Migrating to new navigation types.

## Topics

### Getting built-in navigation view styles

static var automatic: DefaultNavigationViewStyle

The default navigation view style in the current context of the view being styled.

static var columns: ColumnNavigationViewStyle

A navigation view style represented by a series of views in columns.

static var stack: StackNavigationViewStyle

A navigation view style represented by a view stack that only shows a single top view at a time.

### Supporting types

struct DefaultNavigationViewStyle

The default navigation view style.

struct ColumnNavigationViewStyle

A navigation view style represented by a series of views in columns.

struct StackNavigationViewStyle

A navigation view style represented by a view stack that only shows a single top view at a time.

struct DoubleColumnNavigationViewStyle

A navigation view style represented by a primary view stack that navigates to a detail view.

## Relationships

### Conforming Types

- ColumnNavigationViewStyle
- DefaultNavigationViewStyle
- DoubleColumnNavigationViewStyle
- StackNavigationViewStyle

## See Also

### Styling navigation views

func navigationViewStyle&lt;S>(S) -> some View

Sets the style for navigation views within this view.

Deprecated

