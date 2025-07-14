

- SwiftUI
- View fundamentals
- View
-  Auxiliary view modifiers 

API Collection

# Auxiliary view modifiers

Add and configure supporting views, like toolbars and context menus.

## Overview

Use these modifiers to manage supplemental views that present context-specific controls and information. For example, you can add titles and buttons to navigation bars, manage the status bar, create context menus, and add badges many different kinds of views.

## Topics

### Navigation titles

Configure your apps navigation titles

Use a navigation title to display the current navigation state of an interface.

func navigationTitle(_:)

Configures the view’s title for purposes of navigation, using a string binding.

func navigationSubtitle(_:)

Configures the view’s subtitle for purposes of navigation.

### Navigation title configuration

func navigationDocument(_:)

Configures the view’s document for purposes of navigation.

func navigationDocument(_:preview:)

Configures the view’s document for purposes of navigation.

### Navigation bars

func navigationBarBackButtonHidden(Bool) -> some View

Hides the navigation bar back button for the view.

func navigationBarTitleDisplayMode(NavigationBarItem.TitleDisplayMode) -> some View

Configures the title display mode for this view.

### Navigation stacks and columns

func navigationDestination&lt;D, C>(for: D.Type, destination: (D) -> C) -> some View

Associates a destination view with a presented data type for use within a navigation stack.

func navigationDestination&lt;V>(isPresented: Binding&lt;Bool>, destination: () -> V) -> some View

Associates a destination view with a binding that can be used to push the view onto a NavigationStack.

func navigationDestination&lt;D, C>(item: Binding&lt;Optional&lt;D>>, destination: (D) -> C) -> some View

Associates a destination view with a bound value for use within a navigation stack or navigation split view

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

### Tab views

func tabViewCustomization(Binding&lt;TabViewCustomization>?) -> some View

Specifies the customizations to apply to the sidebar representation of the tab view.

func defaultAdaptableTabBarPlacement(AdaptableTabBarPlacement) -> some View

Specifies the default placement for the tabs in a tab view using the adaptable sidebar style.

func tabViewSidebarHeader&lt;Content>(content: () -> Content) -> some View

Adds a custom header to the sidebar of a tab view.

func tabViewSidebarFooter&lt;Content>(content: () -> Content) -> some View

Adds a custom footer to the sidebar of a tab view.

func tabViewSidebarBottomBar&lt;Content>(content: () -> Content) -> some View

Adds a custom bottom bar to the sidebar of a tab view.

func sectionActions&lt;Content>(content: () -> Content) -> some View

Adds custom actions to a section.

### Toolbars

For information about toolbars, see Toolbars.

func toolbar(content:)

Populates the toolbar or navigation bar with the specified items.

func toolbar&lt;Content>(id: String, content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items, allowing for user customization.

func toolbar(Visibility, for: ToolbarPlacement...) -> some View

Specifies the visibility of a bar managed by SwiftUI.

func toolbar(removing: ToolbarDefaultItemKind?) -> some View

Remove a toolbar item present by default

func toolbarVisibility(Visibility, for: ToolbarPlacement...) -> some View

Specifies the visibility of a bar managed by SwiftUI.

func toolbarBackground(_:for:)

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

func toolbarBackgroundVisibility(Visibility, for: ToolbarPlacement...) -> some View

Specifies the preferred visibility of backgrounds on a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarRole(ToolbarRole) -> some View

Configures the semantic role for the content populating the toolbar.

func toolbarTitleMenu&lt;C>(content: () -> C) -> some View

Configure the title menu of a toolbar.

func toolbarTitleDisplayMode(ToolbarTitleDisplayMode) -> some View

Configures the toolbar title display mode for this view.

func ornament&lt;Content>(visibility: Visibility, attachmentAnchor: OrnamentAttachmentAnchor, contentAlignment: Alignment, ornament: () -> Content) -> some View

Presents an ornament.

### Context menus

For information about menus in your app, see Menus and commands.

func contextMenu&lt;MenuItems>(menuItems: () -> MenuItems) -> some View

Adds a context menu to a view.

func contextMenu&lt;M, P>(menuItems: () -> M, preview: () -> P) -> some View

Adds a context menu with a custom preview to a view.

func contextMenu&lt;I, M>(forSelectionType: I.Type, menu: (Set&lt;I>) -> M, primaryAction: ((Set&lt;I>) -> Void)?) -> some View

Adds an item-based context menu to a view.

### Badges

func badge(_:)

Generates a badge for the view from an integer value.

func badgeProminence(BadgeProminence) -> some View

Specifies the prominence of badges created by this view.

### Help text

func help(_:)

Adds help text to a view using a text view that you provide.

### Status bar

func statusBarHidden(Bool) -> some View

Sets the visibility of the status bar.

### Touch Bar

func touchBar&lt;Content>(content: () -> Content) -> some View

Sets the content that the Touch Bar displays.

func touchBar&lt;Content>(TouchBar&lt;Content>) -> some View

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

func touchBarItemPrincipal(Bool) -> some View

Sets principal views that have special significance to this Touch Bar.

func touchBarCustomizationLabel(Text) -> some View

Sets a user-visible string that identifies the view’s functionality.

func touchBarItemPresence(TouchBarItemPresence) -> some View

Sets the behavior of the user-customized view.

## See Also

### Configuring view elements

Accessibility modifiers

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Appearance modifiers

Configure a view’s foreground and background styles, controls, and visibility.

Text and symbol modifiers

Manage the rendering, selection, and entry of text in your view.

Chart view modifiers

Configure charts that you declare with Swift Charts.

