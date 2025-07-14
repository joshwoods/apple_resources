

- SwiftUI
- TabContent
-  accessibilityLabel(\_:isEnabled:) 

Instance Method

# accessibilityLabel(\_:isEnabled:)

Adds a label to the tab that describes its contents.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityLabel(
    _ label: Text,
    isEnabled: Bool = true
) -> some TabContent
```

Show all declarations

## Parameters 

`label`  

The accessibility label to apply.

`isEnabled`  

If true the accessibility label is applied; otherwise the accessibility label is unchanged.

## Discussion

Use this method to provide an accessibility label for a tab that contains content like an icon. Don’t include text in the label that repeats information that users already have. For example, don’t use the label “Library tab” because a tab already has a trait that identifies it as a tab.

```
var body: some View {
    TabView {
        Tab {
            FavoritesView()
        } label: {
            Image(systemName: "star.fill")
        }
        .accessibilityLabel("Favorites")
    }
}
```

