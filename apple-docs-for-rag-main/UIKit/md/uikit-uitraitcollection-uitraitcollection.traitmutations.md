

- UIKit
- UITraitCollection
-  UITraitCollection.TraitMutations 

Type Alias

# UITraitCollection.TraitMutations

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
typealias TraitMutations = (inout any UIMutableTraits) -> Void
```

## See Also

### Modifying traits

convenience init(mutations: (inout any UIMutableTraits) -> Void)

func modifyingTraits((inout any UIMutableTraits) -> Void) -> UITraitCollection

