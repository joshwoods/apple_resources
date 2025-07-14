

- RealityKit
- RealityView
-  listSectionSpacing(\_:) 

Instance Method

# listSectionSpacing(\_:)

Sets the spacing between adjacent sections in a `List`.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystvisionOSwatchOS 10.0+

``` source
nonisolated
func listSectionSpacing(_ spacing: ListSectionSpacing) -> some View
```

## Parameters 

`spacing`  

The `ListSectionSpacing` to apply.

## Discussion

Pass `.default` for the default spacing, or use `.compact` for a compact appearance between sections.

The following example creates a `List` with compact spacing between sections:

```
List {
    Section("Colors") {
        Text("Blue")
        Text("Red")
    }

    Section("Shapes") {
        Text("Square")
        Text("Circle")
    }
}
.listSectionSpacing(.compact)
```

Spacing can also be specified on an individual `Section`, as in this example:

```
Section("Borders") {
    Text("Dashed")
    Text("Solid")
}
.listSectionSpacing(.compact)
```

Spacing applied on sections in the `List` overrides spacing applied on the `List` as a whole.

