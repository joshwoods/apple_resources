

- Contacts UI
- CNContactViewControllerDelegate
-  contactViewController(\_:didCompleteWith:) 

Instance Method

# contactViewController(\_:didCompleteWith:)

Called when the view has been presented.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func contactViewController(
    _ viewController: CNContactViewController,
    didCompleteWith contact: CNContact?
)
```

## Parameters 

`viewController`  

The view controller presenting the contact.

`contact`  

The newly, or existing contact being added.

## Discussion

If creating a new contact, the new contact added to the contacts list is passed in `contact`. If adding to an existing contact, the existing contact is passed in `contact`. It is up to the delegate to dismiss the view controller.

## See Also

### Responding to User Events

func contactViewController(CNContactViewController, shouldPerformDefaultActionFor: CNContactProperty) -> Bool

Called when the user selects a property.

