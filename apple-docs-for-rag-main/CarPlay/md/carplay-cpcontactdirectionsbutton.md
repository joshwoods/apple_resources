

- CarPlay
-  CPContactDirectionsButton 

Class

# CPContactDirectionsButton

A button for getting directions to the contact’s location.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPContactDirectionsButton
```

## Overview

Use this button to get directions to the location of the template’s contact.

If your app doesn’t provide turn-by-turn navigation, use the `maps` URL scheme to launch the most recent navigation app. Call your template application scene’s open(_:options:completionHandler:) method and pass a URL that embeds the contact’s location. CarPlay provides this scene to your CPTemplateApplicationSceneDelegate when the scene connects.

## Topics

### Creating a Contact Directions Button

init(handler: ((CPButton) -> Void)?)

Creates a button that invokes a handler when the user taps it.

## Relationships

### Inherits From

- CPButton

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing Interactions with the Contact

var actions: [CPButton]?

The actions that the template displays for this contact.

class CPContactCallButton

A button for calling the contact.

class CPContactMessageButton

A button that activates Siri and initiates the compose message flow.

