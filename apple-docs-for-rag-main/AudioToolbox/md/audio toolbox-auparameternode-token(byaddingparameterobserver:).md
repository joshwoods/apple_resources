

- Audio Toolbox
- AUParameterNode
-  token(byAddingParameterObserver:) 

Instance Method

# token(byAddingParameterObserver:)

Adds an observer for a single parameter or all parameters in a group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func token(byAddingParameterObserver observer: @escaping AUParameterObserver) -> AUParameterObserverToken
```

## Parameters 

`observer`  

A block called after the value of a parameter has changed.

## Return Value

A token which can be passed to the removeParameterObserver(_:) or setValue(_:originator:) methods.

## Discussion

An audio unit view can use an observer to be notified of changes to a single parameter or all parameters in a group. These callbacks are throttled so as to limit the rate of redundant notifications in the case of frequent changes to a single parameter.

This block is called in an arbitrary thread context and it is responsible for thread-safety. It must not make any calls to add or remove other observers, including itself, as this will deadlock.

An audio unit should interact with the parameter node via the implementorValueObserver and implementorValueProvider properties.

## See Also

### Observers

func token(byAddingParameterRecordingObserver: AUParameterRecordingObserver) -> AUParameterObserverToken

Adds a recording observer for a single parameter or all parameters in a group.

func token(byAddingParameterAutomationObserver: AUParameterAutomationObserver) -> AUParameterObserverToken

func removeParameterObserver(AUParameterObserverToken)

Remove a specific parameter observer.

