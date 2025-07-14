

- RealityKit
- RealityViewDefaultPlaceholder
-  listRowSpacing(\_:) 

Instance Method

# listRowSpacing(\_:)

Sets the vertical spacing between two adjacent rows in a List.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

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

