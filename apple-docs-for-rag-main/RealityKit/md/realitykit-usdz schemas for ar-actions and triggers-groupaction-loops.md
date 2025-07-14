

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- GroupAction
-  loops 

Article

# loops

A Boolean value indicating whether the group loops.

## Overview

The default value is `false`, in which the group executes its actions performCount number of times and then stops.

When `true` and type is `serial`, the group restarts its action sequence with the first action after the last action completes. When type is `parallel`, the runtime repeats each action independently.

### Declaration

```
uniform bool loops = false
```

## See Also

### Properties

info:id

The action’s unique identifier.

type

An option that controls the order in which the actions execute.

performCount

A value that specifies the number of times the group’s actions repeat.

actions

A list of actions that make up the group.

