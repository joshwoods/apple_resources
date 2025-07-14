

- FamilyControls
- FamilyActivityPicker
-  badge(\_:) 

Instance Method

# badge(\_:)

Generates a badge for the view from a localized string key.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
nonisolated
func badge(_ key: LocalizedStringKey?) -> some View
```

## Parameters 

`key`  

An optional string key to display as a badge. Set the value to `nil` to hide the badge.

## Discussion

Use a badge to convey optional, supplementary information about a view. Keep the contents of the badge as short as possible. Badges appear only in list rows, tab bars, and menus.

This modifier creates a `Text` view on your behalf, and treats the localized key similar to `Text/init(_:tableName:bundle:comment:)`. For more information about localizing strings, see `Text`. The following example shows a list with a “Default” badge on one of its rows.

```
NavigationView {
    List(servers) { server in
        Text(server.name)
            .badge(server.isDefault ? "Default" : nil)
    }
    .navigationTitle("Servers")
}
```

## See Also

### Badges

func badge(Int) -> some View

Generates a badge for the view from an integer value.

func badge&lt;S>(S?) -> some View

Generates a badge for the view from a string.

func badge(Text?) -> some View

Generates a badge for the view from a text view.

