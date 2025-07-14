

- SwiftUI
- NavigationViewStyle
-  automatic Deprecated

Type Property

# automatic

The default navigation view style in the current context of the view being styled.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 7.0–11.4Deprecated

``` source
static var automatic: DefaultNavigationViewStyle { get }
```

Available when `Self` is `DefaultNavigationViewStyle`.

Deprecated

Replace a styled NavigationView with a NavigationStack or NavigationSplitView. For more information, see Migrating to new navigation types.

## See Also

### Getting built-in navigation view styles

static var columns: ColumnNavigationViewStyle

A navigation view style represented by a series of views in columns.

Deprecated

static var stack: StackNavigationViewStyle

A navigation view style represented by a view stack that only shows a single top view at a time.

Deprecated

