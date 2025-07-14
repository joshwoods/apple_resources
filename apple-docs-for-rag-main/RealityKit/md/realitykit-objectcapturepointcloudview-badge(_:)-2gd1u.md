

- RealityKit
- ObjectCapturePointCloudView
-  badge(\_:) 

Instance Method

# badge(\_:)

Generates a badge for the view from an integer value.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+

``` source
nonisolated
func badge(_ count: Int) -> some View
```

## Parameters 

`count`  

An integer value to display in the badge. Set the value to zero to hide the badge.

## Discussion

Use a badge to convey optional, supplementary information about a view. Keep the contents of the badge as short as possible. Badges appear only in list rows, tab bars, and menus.

The following example shows a `List` with the value of `recentItems.count` represented by a badge on one of the rows:

```
List {
    Text("Recents")
        .badge(recentItems.count)
    Text("Favorites")
}
```

