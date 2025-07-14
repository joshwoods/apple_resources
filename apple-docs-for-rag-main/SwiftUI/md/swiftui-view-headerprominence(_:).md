

- SwiftUI
- View
-  headerProminence(\_:) 

Instance Method

# headerProminence(\_:)

Sets the header prominence for this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func headerProminence(_ prominence: Prominence) -> some View
```

## Parameters 

`prominence`  

The prominence to apply.

## Discussion

In the following example, the section header appears with increased prominence:

```
List {
    Section(header: Text("Header")) {
        Text("Row")
    }
    .headerProminence(.increased)
}
.listStyle(.insetGrouped)
```

## See Also

### Configuring headers

var headerProminence: Prominence

The prominence to apply to section headers within a view.

enum Prominence

A type indicating the prominence of a view hierarchy.

var defaultMinListHeaderHeight: CGFloat?

The default minimum height of a header in a list.

