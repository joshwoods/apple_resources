

- UIKit
- UIFocusEnvironment
-  soundIdentifierForFocusUpdate(in:) 

Instance Method

# soundIdentifierForFocusUpdate(in:)

Asks the delegate for the identifier of the sound to play when the object gains focus.

tvOS 11.0+

``` source
@MainActor
optional func soundIdentifierForFocusUpdate(in context: UIFocusUpdateContext) -> UIFocusSoundIdentifier?
```

## Parameters 

`context`  

The context object associated with the update.

## Return Value

The identifier of the sound to be played. Return `nil` if you want to let the parent focus environment determine which sound to play.

## Mentioned in 

Using custom sounds for focus movement

## Discussion

Use this method to return a custom sound when the focus environment object gains focus. Return default to play the default system sound, or return none to avoid playing a sound altogether. If you previously registered custom sounds using the register(_:forSoundIdentifier:) method of UIFocusSystem, you may also return an identifier for a sound that you registered.

If you do not implement this method, the system assumes a `nil` return value. If no ancestor environment defines a custom sound, the system plays the default sound.

Important

You must register custom sounds before returning the associated identifiers from this method. Returning an identifier that is unknown to UIKit will result in an assertion failure and an immediate crash.

## See Also

### Getting the sound to play during updates

Using custom sounds for focus movement

Customize the sounds users hear when focus moves.

struct UIFocusSoundIdentifier

An identifier for a focus-related sound.

