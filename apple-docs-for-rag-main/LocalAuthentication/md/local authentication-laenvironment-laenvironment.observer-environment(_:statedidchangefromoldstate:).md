

- Local Authentication
- LAEnvironment
- LAEnvironment.Observer
-  environment(\_:stateDidChangeFromOldState:) 

Instance Method

# environment(\_:stateDidChangeFromOldState:)

Called when there has been a change in the environment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
optional func environment(
    _ environment: LAEnvironment,
    stateDidChangeFromOldState oldState: LAEnvironment.State
)
```

## Parameters 

`oldState`  

The old environment state (before update)

## Discussion

Invoked on a queue private to LocalAuthentication framework. At the moment of invocation of this method, @c LAEnvironment.state already contains the new updated state.

