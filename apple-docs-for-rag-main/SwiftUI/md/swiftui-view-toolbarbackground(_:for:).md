

- SwiftUI
- View
-  toolbarBackground(\_:for:) 

Instance Method

# toolbarBackground(\_:for:)

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func toolbarBackground(
    _ style: S,
    for bars: ToolbarPlacement...
) -> some View where S : ShapeStyle
```

Show all declarations

## Parameters 

`style`  

The style to display as the background of the bar.

`bars`  

The bars to use the style for or automatic if empty.

## Discussion

The preferred style flows up to the nearest container that renders a bar. This could be a NavigationView or TabView in iOS, or the root view of a WindowGroup in macOS. This example shows a view that renders the navigation bar with a blue background and dark color scheme.

```
NavigationView {
    ContentView()
        .toolbarBackground(.white)
        .toolbarColorScheme(.dark)
}
```

You can provide multiple ToolbarPlacement instances to customize multiple bars at once.

```
TabView {
    NavigationView {
        ContentView()
            .toolbarBackground(
                .blue, for: .navigationBar, .tabBar)
            .toolbarColorScheme(
                .dark, for: .navigationBar, .tabBar)
    }
}
```

When used within a TabView, the specified style will be preferred while the tab is currently active. You can use a Group to specify the same preferred background for every tab.

```
TabView {
    Group {
        MainView()
        SettingsView()
    }
    .toolbarBackground(.blue, for: .tabBar)
}
```

Depending on the specified bars, the requested style may not be able to be fullfilled.

## See Also

### Styling a toolbar

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

func windowToolbarStyle&lt;S>(S) -> some Scene

Sets the style for the toolbar defined within this scene.

protocol WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

var toolbarLabelStyle: ToolbarLabelStyle?

The label style to apply to controls within a toolbar.

struct ToolbarLabelStyle

The label style of a toolbar.

