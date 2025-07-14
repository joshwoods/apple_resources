

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- Preliminary_Behavior
-  exclusive 

Article

# exclusive

A Boolean value that determines if a behavior executes exclusively.

## Overview

The default value is `false`, which indicates that other behaviors’ actions run concurrently with the behavior. If the value is `true`, other exclusive behaviors stop performing actions when the runtime actives a trigger in the behavior.

### Declaration

```
uniform bool exclusive = false
```

## See Also

### Properties

triggers

A list of prims that execute a behavior’s actions.

actions

A list of actions that make up the group.

