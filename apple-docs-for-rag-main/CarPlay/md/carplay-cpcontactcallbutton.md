

- CarPlay
-  CPContactCallButton 

Class

# CPContactCallButton

A button for calling the contact.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPContactCallButton
```

## Overview

Use this button to call the template’s contact.

If your app doesn’t provide VoIP functionality, use the `tel` URL scheme to start a phone call with the contact. Invoke your template application scene’s open(_:options:completionHandler:) method and pass the URL. CarPlay provides this scene to your CPTemplateApplicationSceneDelegate when the scene connects.

## Topics

### Creating a Contact Call Button

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

class CPContactDirectionsButton

A button for getting directions to the contact’s location.

class CPContactMessageButton

A button that activates Siri and initiates the compose message flow.

