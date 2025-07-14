

- Address Book UI
-  ABUnknownPersonViewControllerDelegate Deprecated

Protocol

# ABUnknownPersonViewControllerDelegate

The methods you use to respond to events in an unknown person view controller.

iOS 2.0+iPadOS 2.0+Mac Catalyst 14.0+

``` source
protocol ABUnknownPersonViewControllerDelegate : NSObjectProtocol
```

Deprecated

Use CNContactViewController instead.

## Topics

### Responding to User Events

func unknownPersonViewController(ABUnknownPersonViewController, didResolveToPerson: ABRecord?)

Sent when the user finishes creating a contact or adding the displayed person properties to an existing contact.

**Required**

func unknownPersonViewController(ABUnknownPersonViewController, shouldPerformDefaultActionForPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects a property value of the person displayed in a person view controller.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to View Controller Interactions

var unknownPersonViewDelegate: (any ABUnknownPersonViewControllerDelegate)?

The unknown-person view controller delegate.

Deprecated

