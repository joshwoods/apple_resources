

- SwiftUI
- HoverEffectGroup
- HoverEffectGroup.Behavior
-  ignoresGroup 

Type Property

# ignoresGroup

Ignores the current phase of the match group.

visionOS 2.0+

``` source
static let ignoresGroup: HoverEffectGroup.Behavior
```

## Discussion

Use this behavior when an effect should should neither activate a group, or become activated by any other effect in the group. The effect will only become active when directly hovered.

