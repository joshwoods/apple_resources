

- Audio Toolbox
- AUParameterNode
-  removeParameterObserver(\_:) 

Instance Method

# removeParameterObserver(\_:)

Remove a specific parameter observer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeParameterObserver(_ token: AUParameterObserverToken)
```

## Parameters 

`token`  

The token corresponding to the given observer.

## Discussion

This call will remove the callback corresponding to the given token. This operation blocks until any callbacks currently in progress have completed.

## See Also

### Observers

func token(byAddingParameterObserver: AUParameterObserver) -> AUParameterObserverToken

Adds an observer for a single parameter or all parameters in a group.

func token(byAddingParameterRecordingObserver: AUParameterRecordingObserver) -> AUParameterObserverToken

Adds a recording observer for a single parameter or all parameters in a group.

func token(byAddingParameterAutomationObserver: AUParameterAutomationObserver) -> AUParameterObserverToken

