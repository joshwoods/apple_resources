

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- AudioAction
-  type 

Article

# type

An option that controls the order in which the actions execute.

## Overview

The default value is `serial`.

### Order Options

`serial`  
Executes in order with each action waiting for the prior action to complete before starting.

`parallel`  
Executes all actions concurrently.

### Declaration

```
uniform token type = "serial" (
        allowedTokens = ["serial", "parallel"]
)
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

audio

The location of an audio file.

gain

A value that controls the audio volume.

auralMode

An option that controls the audio signal’s spacial dynamics.

