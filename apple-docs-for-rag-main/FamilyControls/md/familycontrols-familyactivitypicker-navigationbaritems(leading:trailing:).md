

- FamilyControls
- FamilyActivityPicker
-  navigationBarItems(leading:trailing:) 

Instance Method

# navigationBarItems(leading:trailing:)

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+

``` source
nonisolated
func navigationBarItems(
    leading: L,
    trailing: T
) -> some View where L : View, T : View
```

## See Also

### Deprecated Auxiliary View Modifiers

func navigationBarTitle&lt;S>(S) -> some View

Sets the title of this view’s navigation bar with a string.

func navigationBarTitle(LocalizedStringKey) -> some View

Sets the title of this view’s navigation bar with a localized string.

func navigationBarTitle(Text) -> some View

Sets the title in the navigation bar for this view.

func navigationBarTitle(Text, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarTitle&lt;S>(S, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarTitle(LocalizedStringKey, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarItems&lt;L>(leading: L) -> some View

func navigationBarItems&lt;T>(trailing: T) -> some View

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

