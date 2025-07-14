

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- Preliminary_Action
-  multiplePerformOperation 

Article

# multiplePerformOperation

An option that indicates how an action handles an additional invocation while running.

## Overview

The runtime doesn’t react to this property for all actions.

### Additional Invocation Options

`allow`  
Restarts the action by playing it over again.

`ignore`  
Continues running the current action, ignoring the additional invocation.

`stop`  
Stops the current action.

### Declaration

```
uniform token multiplePerformOperation= "ignore" (
    allowedTokens = ["ignore", "allow", "stop"]
)
```

## See Also

### Properties

info:id

The action’s unique identifier.

