

- Create ML Components
- JointsSelector
-  init(ignoredJoints:) 

Initializer

# init(ignoredJoints:)

Creates a joint selector transformer using a list of joint keys to be ignored.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(ignoredJoints: [JointKey])
```

## Parameters 

`ignoredJoints`  

Joint keys to be ignored and set to zero in the pose.

## See Also

### Creating a selector

init(selectedJoints: [JointKey])

Creates a joint selector transformer using a list of joint keys to be selected.

