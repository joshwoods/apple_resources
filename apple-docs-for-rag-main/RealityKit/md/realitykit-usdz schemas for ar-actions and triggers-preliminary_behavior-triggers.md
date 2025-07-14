

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- Preliminary_Behavior
-  triggers 

Article

# triggers

A list of prims that execute a behavior’s actions.

## Overview

The runtime executes all actions in the actions array if the conditions of any trigger in triggers are satisfied. Only insert Preliminary_Trigger prims in this array.

### Declaration

```
rel triggers
```

## See Also

### Properties

actions

A list of actions that make up the group.

exclusive

A Boolean value that determines if a behavior executes exclusively.

