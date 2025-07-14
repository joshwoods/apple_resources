

- Create ML Components
- JointsSelector
-  init(selectedJoints:) 

Initializer

# init(selectedJoints:)

Creates a joint selector transformer using a list of joint keys to be selected.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(selectedJoints: [JointKey])
```

## Parameters 

`selectedJoints`  

Joint keys to be selected from the pose.

## See Also

### Creating a selector

init(ignoredJoints: [JointKey])

Creates a joint selector transformer using a list of joint keys to be ignored.

