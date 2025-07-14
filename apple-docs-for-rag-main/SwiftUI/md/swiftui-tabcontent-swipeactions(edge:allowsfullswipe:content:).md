

- SwiftUI
- TabContent
-  swipeActions(edge:allowsFullSwipe:content:) 

Instance Method

# swipeActions(edge:allowsFullSwipe:content:)

Adds custom swipe actions to a tab in a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func swipeActions(
    edge: HorizontalEdge = .trailing,
    allowsFullSwipe: Bool = true,
    @ViewBuilder content: () -> T
) -> some TabContent where T : View
```

## Parameters 

`edge`  

The edge of the view to associate the swipe actions with. The default is HorizontalEdge.trailing.

`allowsFullSwipe`  

A Boolean value that indicates whether a full swipe automatically performs the first action. The default is `true`.

`content`  

The content of the swipe actions.

## Discussion

Use this method to add swipe actions to a view that acts as a row in the tab sidebar. Indicate the HorizontalEdge where the swipe action originates, and define individual actions with Button instances. For example, if you have a group of message categories, you can add an action to toggle a category as unread on a swipe from the leading edge, and actions to hide or flag categories on a trailing edge swipe:

```
TabView {
     TabSection("Messages") {
         ForEach(store.messageCategories) { category in
             Tab(category.title, image: category.image)
                 .swipeActions(edge: .leading) {
                     Button { store.toggleUnread(category) } label: {
                         if category.isUnread {
                             Label("Read", systemImage: "envelope.open")
                         } else {
                             Label("Unread", systemImage: "envelope.badge")
                         }
                     }
                 }
                 .swipeActions(edge: .trailing) {
                     Button(role: .destructive) {
                         store.hide(category)
                     } label: {
                         Label("Remove", systemImage: "trash")
                     }
                     Button { store.flag(category) } label: {
                         Label("Flag", systemImage: "flag")
                     }
                 }
             }
         }
     }
}
```

Actions appear in the order you list them, starting from the swipe’s originating edge. In the example above, the Delete action appears closest to the screen’s trailing edge.

For labels or images that appear in swipe actions, SwiftUI automatically applies the fill symbol variant, as shown above.

By default, the user can perform the first action for a given swipe direction with a full swipe. For the example above, the user can perform both the toggle unread and delete actions with full swipes. You can opt out of this behavior for an edge by setting the `allowsFullSwipe` parameter to `false`. For example, you can disable the full swipe on the leading edge:

```
.swipeActions(edge: .leading, allowsFullSwipe: false) {
    Button { store.toggleUnread(category) } label: {
        if category.isUnread {
            Label("Read", systemImage: "envelope.open")
        } else {
            Label("Unread", systemImage: "envelope.badge")
        }
    }
}
```

When you set a role for a button using one of the values from the ButtonRole enumeration, SwiftUI styles the button according to its role. In the example above, the delete action appears in red because it has the destructive role. If you want to set a different color — for example, to match the overall theme of your app’s UI — add the tint(_:) modifier to the button:

```
.swipeActions(edge: .leading) {
    Button { store.toggleUnread(category) } label: {
        if category.isUnread {
            Label("Read", systemImage: "envelope.open")
        } else {
            Label("Unread", systemImage: "envelope.badge")
        }
    }
    .tint(.blue)
}
.swipeActions(edge: .trailing) {
    Button(role: .destructive) { store.hide(category) } label: {
        Label("Hide", systemImage: "trash")
    }
    Button { store.flag(category) } label: {
        Label("Flag", systemImage: "flag")
    }
    .tint(.orange)
}
```

The modifications in the code above make the toggle unread action blue and the flag action orange:

Actions accumulate for a given edge if you call the modifier multiple times on the same tab.

