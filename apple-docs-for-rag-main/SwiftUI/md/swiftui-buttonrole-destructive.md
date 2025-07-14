

- SwiftUI
- ButtonRole
-  destructive 

Type Property

# destructive

A role that indicates a destructive button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let destructive: ButtonRole
```

## Discussion

Use this role for a button that deletes user data, or performs an irreversible operation. A destructive button signals by its appearance that the user should carefully consider whether to tap or click the button. For example, SwiftUI presents a destructive button that you add with the swipeActions(edge:allowsFullSwipe:content:) modifier using a red background:

```
List {
    ForEach(items) { item in
        Text(item.title)
            .swipeActions {
                Button(role: .destructive) { delete() } label: {
                    Label("Delete", systemImage: "trash")
                }
            }
    }
}
.navigationTitle("Shopping List")
```

## See Also

### Getting button roles

static let cancel: ButtonRole

A role that indicates a button that cancels an operation.

