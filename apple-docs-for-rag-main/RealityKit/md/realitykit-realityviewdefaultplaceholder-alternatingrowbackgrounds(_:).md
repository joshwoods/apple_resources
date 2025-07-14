

- RealityKit
- RealityViewDefaultPlaceholder
-  alternatingRowBackgrounds(\_:) 

Instance Method

# alternatingRowBackgrounds(\_:)

Overrides whether lists and tables in this view have alternating row backgrounds.

RealityKitSwiftUImacOS 14.0+

``` source
nonisolated
func alternatingRowBackgrounds(_ behavior: AlternatingRowBackgroundBehavior = .enabled) -> some View
```

## Parameters 

`behavior`  

Whether alternating row backgrounds are enabled or not.

## Discussion

This can be used in conjunction with an explicit list or table style or used by itself to customize the row backgrounds of the automatic style. The only list style this has no effect on is `.sidebar.`

```
List(recipe.ingredients) {
    Text($0.name)
}
.listStyle(.bordered)
.alternatingRowBackgrounds()
```

This is able to be combined with `scrollContentBackground(_:)` and applies an alternating row background on top of the overall list or table background.

This can also be combined with `listRowBackground`, which overrides the background for a specific list row, replacing the automatic alternating background for that row.

