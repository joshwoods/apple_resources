

- SwiftUI
- View
-  safeAreaPadding(\_:) 

Instance Method

# safeAreaPadding(\_:)

Adds the provided insets into the safe area of this view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func safeAreaPadding(_ insets: EdgeInsets) -> some View
```

Show all declarations

## Discussion

Use this modifier when you would like to add a fixed amount of space to the safe area a view sees.

```
ScrollView(.horizontal) {
    HStack(spacing: 10.0) {
        ForEach(items) { item in
            ItemView(item)
        }
    }
}
.safeAreaPadding(.horizontal, 20.0)
```

See the `View/safeAreaInset(edge:alignment:spacing:content)` modifier for adding to the safe area based on the size of a view.

## See Also

### Staying in the safe areas

func ignoresSafeArea(SafeAreaRegions, edges: Edge.Set) -> some View

Expands the safe area of a view.

func safeAreaInset(edge:alignment:spacing:content:)

Shows the specified content beside the modified view.

func safeAreaPadding(Edge.Set, CGFloat?) -> some View

Adds the provided insets into the safe area of this view.

struct SafeAreaRegions

A set of symbolic safe area regions.

