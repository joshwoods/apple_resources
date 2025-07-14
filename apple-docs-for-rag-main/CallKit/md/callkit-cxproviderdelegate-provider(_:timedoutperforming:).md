

- CallKit
- CXProviderDelegate
-  provider(\_:timedOutPerforming:) 

Instance Method

# provider(\_:timedOutPerforming:)

Called when the provider performs the specified action times out.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
optional func provider(
    _ provider: CXProvider,
    timedOutPerforming action: CXAction
)
```

## Parameters 

`provider`  

The telephony provider.

`action`  

The action that timed out.

## Discussion

Depending on the action, a timeout may also force the call to end.

An action that has already timed out should not be fulfilled or failed by the provider delegate.

## See Also

### Handling Call Actions

func provider(CXProvider, perform: CXStartCallAction)

Called when the provider performs the specified start call action.

func provider(CXProvider, perform: CXAnswerCallAction)

Called when the provider performs the specified answer call action.

func provider(CXProvider, perform: CXEndCallAction)

Called when the provider performs the specified end call action.

func provider(CXProvider, perform: CXSetHeldCallAction)

Called when the provider performs the specified set held call action.

func provider(CXProvider, perform: CXSetMutedCallAction)

Called when the provider performs the specified set muted call action.

func provider(CXProvider, perform: CXSetGroupCallAction)

Called when the provider performs the specified set group call action.

func provider(CXProvider, perform: CXPlayDTMFCallAction)

Called when the provider performs the specified play DTMF (dual tone multifrequency) call action.

