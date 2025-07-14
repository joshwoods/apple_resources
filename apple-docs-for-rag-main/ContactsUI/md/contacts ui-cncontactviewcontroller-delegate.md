

- Contacts UI
- CNContactViewController
-  delegate 

Instance Property

# delegate

The delegate to be notified.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any CNContactViewControllerDelegate)? { get set }
```

## Discussion

The notification is sent when the user selects a property, or when the contact view controller is dismissed by its parent.

## See Also

### Handling Interactions with the Interface

protocol CNContactViewControllerDelegate

Methods you use to respond to user interactions with a contact view controller.

