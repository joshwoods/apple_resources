

- ManagedAppDistribution
- ManagedContentView
-  navigationTitle(\_:) 

Instance Method

# navigationTitle(\_:)

Configures the view’s title for purposes of navigation, using a custom view.

ManagedAppDistributionSwiftUIwatchOS 7.0+

``` source
nonisolated
func navigationTitle(@ViewBuilder _ title: () -> V) -> some View where V : View
```

## Parameters 

`title`  

The view to display.

## Discussion

A view’s navigation title is used to visually display the current navigation state of an interface. On iOS and watchOS, when a view is navigated to inside of a navigation view, that view’s title is displayed in the navigation bar. On iPadOS, the primary destination’s navigation title is reflected as the window’s title in the App Switcher. Similarly on macOS, the primary destination’s title is used as the window title in the titlebar, Windows menu and Mission Control.

