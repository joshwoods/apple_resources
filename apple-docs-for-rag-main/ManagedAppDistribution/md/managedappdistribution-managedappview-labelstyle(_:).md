

- ManagedAppDistribution
- ManagedAppView
-  labelStyle(\_:) 

Instance Method

# labelStyle(\_:)

Sets the style for labels within this view.

ManagedAppDistributionSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func labelStyle(_ style: S) -> some View where S : LabelStyle
```

## Discussion

Use this modifier to set a specific style for all labels within a view:

```
VStack {
    Label("Fire", systemImage: "flame.fill")
    Label("Lightning", systemImage: "bolt.fill")
}
.labelStyle(MyCustomLabelStyle())
```

