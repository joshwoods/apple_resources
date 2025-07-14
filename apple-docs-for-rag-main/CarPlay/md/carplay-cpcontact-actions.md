

- CarPlay
- CPContact
-  actions 

Instance Property

# actions

The actions that the template displays for this contact.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var actions: [CPButton]? { get set }
```

## Discussion

Assign an array of CPButton objects to this property to update the action buttons that the template displays for this contact. The template can display four buttons maximum. If the array contains more buttons, the template uses only the first four.

Contact actions are optional, and the default value is nil.

## See Also

### Managing Interactions with the Contact

class CPContactCallButton

A button for calling the contact.

class CPContactDirectionsButton

A button for getting directions to the contact’s location.

class CPContactMessageButton

A button that activates Siri and initiates the compose message flow.

