

- CarPlay
- CPVoiceControlTemplate
-  activateVoiceControlState(withIdentifier:) 

Instance Method

# activateVoiceControlState(withIdentifier:)

Changes the template’s state to the one matching the specified identifier.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func activateVoiceControlState(withIdentifier identifier: String)
```

## Parameters 

`identifier`  

An identifier corresponding to one of the voiceControlStates associated with the template.

## Discussion

Your app must present the voice control template using its CPInterfaceController object before the app can activate a new state. Calling this method before presenting the template has no effect on the active state.

Note

The voice control template applies a rate limit for voice control states, ignoring state changes occurring too rapidly or frequently in a short period of time.

## See Also

### Activating a State

var activeStateIdentifier: String?

The identifier of the template’s current voice control state.

