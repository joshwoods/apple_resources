

- SwiftUI
- View
-  listRowSpacing(\_:) 

Instance Method

# listRowSpacing(\_:)

Sets the vertical spacing between two adjacent rows in a List.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
nonisolated
func listRowSpacing(_ spacing: CGFloat?) -> some View
```

## Parameters 

`spacing`  

The spacing value to use. A value of `nil` uses the default spacing.

## Discussion

The following example creates a List with 10 pts of spacing between each row:

```
List {
    Text("Blue")
    Text("Red")
}
.listRowSpacing(10.0)
```

## See Also

### Configuring spacing

func listSectionSpacing(_:)

Sets the spacing between adjacent sections in a List to a custom value.

struct ListSectionSpacing

The spacing options between two adjacent sections in a list.

