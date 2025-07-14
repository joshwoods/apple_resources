

- SwiftUI
- HoverEffectGroup
-  init(\_:behavior:) 

Initializer

# init(\_:behavior:)

Creates a new HoverEffectGroup from a `Namespace.ID`.

visionOS 2.0+

``` source
init(
    _ namespace: Namespace.ID,
    behavior: HoverEffectGroup.Behavior = .activatesGroup
)
```

## Parameters 

`namespace`  

The namespace that identifies the group.

`behavior`  

How the effect will behave relative to other effects in the group.

## Return Value

A new HoverEffectGroup

