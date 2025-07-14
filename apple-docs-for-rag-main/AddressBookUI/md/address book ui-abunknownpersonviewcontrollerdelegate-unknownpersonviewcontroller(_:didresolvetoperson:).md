

- Address Book UI
- ABUnknownPersonViewControllerDelegate
-  unknownPersonViewController(\_:didResolveToPerson:) 

Instance Method

# unknownPersonViewController(\_:didResolveToPerson:)

Sent when the user finishes creating a contact or adding the displayed person properties to an existing contact.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
func unknownPersonViewController(
    _ unknownCardViewController: ABUnknownPersonViewController,
    didResolveToPerson person: ABRecord?
)
```

**Required**

## Parameters 

`person`  

The contact the user created or to which they added information. This record is saved in the Address Book database.

`NULL` when the user cancelled the interaction.

## See Also

### Responding to User Events

func unknownPersonViewController(ABUnknownPersonViewController, shouldPerformDefaultActionForPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects a property value of the person displayed in a person view controller.

