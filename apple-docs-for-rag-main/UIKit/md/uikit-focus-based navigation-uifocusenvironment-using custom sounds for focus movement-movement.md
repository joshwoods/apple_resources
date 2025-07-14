

- UIKit
- Focus-based navigation
- UIFocusEnvironment
-  Using custom sounds for focus movement 

Article

# Using custom sounds for focus movement

Customize the sounds users hear when focus moves.

## Overview

The default focus movement sounds are sufficient for the vast majority of apps. However, there might be times when you want to change the default sound to a custom sound that’s more suited to your app.

### Add a custom sound file to your app

Drag the custom focus sound file into your Xcode project. Ensure that the app is selected as a target. You can use any sound file that conforms to the standard iOS sound file formats and is less than 30 seconds long. However, be sure that the sounds you create are appropriate for your app. Playing a 20-second sound clip every time the user moves focus won’t result in a good user experience.

### Register your sound file

After you add the sound file to your app, you have to register the sound file with the focus environment. Before registering the sound file, you must create an identifier for the sound using UIFocusSoundIdentifier. The identifier must be unique for the app. After creating an identifier, locate the sound file in your app bundle and register the sound file using register(_:forSoundIdentifier:).

```
let myPing = UIFocusSoundIdentifier.init(rawValue: "customPing")
let soundURL = Bundle.main.url(forResource: "ping", withExtension: "aif")!
UIFocusSystem.register(_: soundURL, forSoundIdentifier: myPing)
```

There are a few things to remember when registering your sound file:

- Register the sound file early in your app’s lifecycle. The cost to prepare a sound for playback is nontrivial, so you want the sound to be fully prepared by the time a focus update occurs.

- You can register multiple sound files in your app.

- Register each sound file once. Registering a previously registered sound file results in an error that causes an immediate assertion failure.

- See the WWDC 2017 video Focus Interaction in tvOS 11 for information about which focus sound is played when an item becomes focused.

### Override the default focus sounds

The soundIdentifierForFocusUpdate(in:) function is called when focus changes. The default focus sound is played when this function isn’t implemented. Override the function to play your custom sounds when focus changes.

```
override func soundIdentifierForFocusUpdate(in context: UIFocusUpdateContext) -> UIFocusSoundIdentifier? {    
    return myPing
}
```

## See Also

### Getting the sound to play during updates

func soundIdentifierForFocusUpdate(in: UIFocusUpdateContext) -> UIFocusSoundIdentifier?

Asks the delegate for the identifier of the sound to play when the object gains focus.

struct UIFocusSoundIdentifier

An identifier for a focus-related sound.

