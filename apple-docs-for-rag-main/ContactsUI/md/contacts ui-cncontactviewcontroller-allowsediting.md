

- Contacts UI
- CNContactViewController
-  allowsEditing 

Instance Property

# allowsEditing

Determines whether the user can edit the contact’s information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsEditing: Bool { get set }
```

## Discussion

By default, the value of this property is true. All properties are visible when editing a contact.

## See Also

### Customizing Contact Card

var allowsActions: Bool

Determines whether to display buttons for actions such as sending a text message or initiating a FaceTime call.

var shouldShowLinkedContacts: Bool

Determines whether to display data from contacts that are linked to the contact being displayed.

