

- Audio Toolbox
- AUParameterNode
-  token(byAddingParameterAutomationObserver:) 

Instance Method

# token(byAddingParameterAutomationObserver:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func token(byAddingParameterAutomationObserver observer: @escaping AUParameterAutomationObserver) -> AUParameterObserverToken
```

## See Also

### Observers

func token(byAddingParameterObserver: AUParameterObserver) -> AUParameterObserverToken

Adds an observer for a single parameter or all parameters in a group.

func token(byAddingParameterRecordingObserver: AUParameterRecordingObserver) -> AUParameterObserverToken

Adds a recording observer for a single parameter or all parameters in a group.

func removeParameterObserver(AUParameterObserverToken)

Remove a specific parameter observer.

