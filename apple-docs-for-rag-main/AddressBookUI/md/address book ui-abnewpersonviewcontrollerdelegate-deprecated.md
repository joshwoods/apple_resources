

- Address Book UI
-  ABNewPersonViewControllerDelegate Deprecated

Protocol

# ABNewPersonViewControllerDelegate

The `ABNewPersonViewControllerDelegate` protocol declares the interface that ABNewPersonViewController delegates must implement.

iOS 2.0+iPadOS 2.0+Mac Catalyst 14.0+

``` source
protocol ABNewPersonViewControllerDelegate : NSObjectProtocol
```

Deprecated

Use CNContactViewControllerDelegate instead.

## Topics

### Responding to User Events

func newPersonViewController(ABNewPersonViewController, didCompleteWithNewPerson: ABRecord?)

Sent when the user taps Save or Cancel. If the user tapped Save, the current address book has been saved to the Address Book database.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to View Controller Interactions

var newPersonViewDelegate: (any ABNewPersonViewControllerDelegate)?

The delegate of a new-person view controller.

Deprecated

