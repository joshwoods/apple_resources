

- CarPlay
- CPVoiceControlTemplate
-  activeStateIdentifier 

Instance Property

# activeStateIdentifier

The identifier of the template’s current voice control state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var activeStateIdentifier: String? { get }
```

## See Also

### Activating a State

func activateVoiceControlState(withIdentifier: String)

Changes the template’s state to the one matching the specified identifier.

