

- CallKit
- CXProviderDelegate
-  provider(\_:perform:) 

Instance Method

# provider(\_:perform:)

Called when the provider performs the specified play DTMF (dual tone multifrequency) call action.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
optional func provider(
    _ provider: CXProvider,
    perform action: CXPlayDTMFCallAction
)
```

## Parameters 

`provider`  

The telephony provider.

`action`  

The play DTMF call action.

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

func provider(CXProvider, timedOutPerforming: CXAction)

Called when the provider performs the specified action times out.

