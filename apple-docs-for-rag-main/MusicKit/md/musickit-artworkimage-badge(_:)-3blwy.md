

- MusicKit
- ArtworkImage
-  badge(\_:) 

Instance Method

# badge(\_:)

Generates a badge for the view from a text view.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
func badge(_ label: Text?) -> some View
```

## Parameters 

`label`  

An optional `Text` view to display as a badge. Set the value to `nil` to hide the badge.

## Discussion

Use a badge to convey optional, supplementary information about a view. Keep the contents of the badge as short as possible. Badges appear only in list rows, tab bars, and menus.

Use this initializer when you want to style a `Text` view for use as a badge. The following example customizes the badge with the `Text/monospacedDigit()`, `Text/foregroundColor(_:)`, and `Text/bold()` modifiers.

```
var body: some View {
    let badgeView = Text("\(recentItems.count)")
        .monospacedDigit()
        .foregroundColor(.red)
        .bold()

    List {
        Text("Recents")
            .badge(badgeView)
        Text("Favorites")
    }
}
```

Styling the text view has no effect when the badge appears in a `TabView`.

