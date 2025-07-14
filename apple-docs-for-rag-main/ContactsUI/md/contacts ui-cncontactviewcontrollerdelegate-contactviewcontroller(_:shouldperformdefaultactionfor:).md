

- Contacts UI
- CNContactViewControllerDelegate
-  contactViewController(\_:shouldPerformDefaultActionFor:) 

Instance Method

# contactViewController(\_:shouldPerformDefaultActionFor:)

Called when the user selects a property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func contactViewController(
    _ viewController: CNContactViewController,
    shouldPerformDefaultActionFor property: CNContactProperty
) -> Bool
```

## Parameters 

`viewController`  

The view controller presenting the contact.

`property`  

The property (CNContactProperty) selected by the user.

## Return Value

true to call the default action performed for the property, otherwise return false.

## Discussion

Implement this method to determine the resulting behavior when a property is selected. Return false if you do not want anything to be done or if you are handling the actions yourself.

## See Also

### Responding to User Events

func contactViewController(CNContactViewController, didCompleteWith: CNContact?)

Called when the view has been presented.

