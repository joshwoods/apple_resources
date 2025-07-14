

- SwiftUI
- HoverEffectGroup
-  init(id:in:behavior:) 

Initializer

# init(id:in:behavior:)

Creates a new HoverEffectGroup.

visionOS 2.0+

``` source
init(
    id: String?,
    in namespace: Namespace.ID,
    behavior: HoverEffectGroup.Behavior = .activatesGroup
)
```

## Parameters 

`id`  

An optional id to give the group. If provided, the group will be uniquely identified by combining the id and the namespace.

`namespace`  

The namespace that identifies the group.

`behavior`  

How the effect will behave relative to other effects in the group.

## Return Value

A new HoverEffectGroup

