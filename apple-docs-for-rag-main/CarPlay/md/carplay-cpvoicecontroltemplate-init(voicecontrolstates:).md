

- CarPlay
- CPVoiceControlTemplate
-  init(voiceControlStates:) 

Initializer

# init(voiceControlStates:)

Creates a voice control template with a list of voice control states.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(voiceControlStates: [CPVoiceControlState])
```

## Parameters 

`voiceControlStates`  

An array of voice control states associated with the template. You can provide up to five states. If you provide more, the template ignores any states after the first five in the array.

## Return Value

A newly initialized voice control template.

## Discussion

When presenting the voice control template for the first time, the template defaults to the first state in the `voiceControlStates` array. You can change the state after presenting the template by calling the activateVoiceControlState(withIdentifier:) method.

## See Also

### Creating a Voice Control Template

class CPVoiceControlState

A voice control state containing title variants and images for use by a voice control template.

